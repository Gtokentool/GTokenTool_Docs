---
description: 我们将介绍如何获取可替代代币（例如 USDC）的所有持有者。这在您想要追踪代币持有者或用空投奖励持有者的情况下非常有用。
---

# 如何在 Solana链上获取代币持有者

## 概述

让我们首先看看代币（尤其是非同质化代币）在 Solana 上是如何运作的。当开发人员创建代币时，他们使用代币程序创建一个铸币账户。这个铸币账户包含有关特定代币的信息，例如名称、代币地址和图像。一旦创建了铸币账户，就可以铸造代币并将其存储在代币账户中。代币账户是一个包含有关特定地址拥有的特定代币的信息的账户。这将包括铸币地址、所有者地址和账户中特定代币的数量等详细信息。例如，持有一些 USDC（SPL 代币）的地址将有一个 USDC 的代币账户。

我们了解了代币和代币账户的工作原理，我们可以看看如何获​​取给定代币的所有代币持有者。每个持有特定代币的钱包都会有一个该代币的代币账户。这意味着此代币将与持有该代币的所有钱包的代币账户相关联。这就是我们找出所有持有者的方法。如果我们能找到一种方法来获取与代币相关联的所有代币账户，然后获取这些账户的所有者，我们就会得到所有持有者的名单！

## getTokenAccounts 方法

幸运的是，Helius getTokenAccounts API 方法允许我们精确地做到这一点。我们能够在 API 调用参数中包含任何代币的铸币地址，我们将获得为该代币创建的所有代币帐户的列表。除此之外，API 还返回每个代币帐户的所有者；这个所有者就是我们通常所说的代币持有者。需要注意的一件小事是，一个帐户可以有多个针对同一代币的代币帐户。这不是什么大问题；我们只需要设置一些逻辑来处理共享所有者的代币帐户。

## 执行

现在让我们深入研究一些代码，看看我们实际上如何做到这一点。您需要一个 Helius API 密钥才能继续操作。您可以前往https://dev.helius.xyz并注册一个帐户，免费获取一个。首先，我们必须创建一个名为getTokenHolders.js的 Javascript 文件。我们可以先添加我们的 Helius URL 并导入 fs 库，将结果保存到JSON文件中。

```

const url = `https://mainnet.helius-rpc.com/?api-key=`;
const fs = require("fs");

```

接下来，我们将创建一种方法来获取与特定代币相关联的所有代币帐户。我们可以首先创建一个名为 findHolders 的方法，该方法将使用 getTokenAccounts 方法获取所需的数据。您可以在此处阅读有关getTokenAccounts方法的更多信息。需要注意的一件重要事情是，每次调用 API 最多只能返回 1000 个代币帐户。Solana 上的大多数大型代币都有超过 100,000 个代币帐户。为了解决这个问题，我们将使用分页浏览所有代币帐户并继续进行 API 调用，直到我们获取与所有现有代币帐户相关的数据。在该方法中，我们将在getTokenAccounts调用的参数中包含代币铸币厂。当我们循环遍历所有代币帐户时，我们会将每个唯一的代币帐户所有者添加到列表中。方法运行完成后，我们会将此列表保存到包含所有代币持有者的JSON文件中。

```

const findHolders = async () => {
  // Pagination logic
  let page = 1;
 	// allOwners will store all the addresses that hold the token
  let allOwners = new Set();

  while (true) {
    const response = await fetch(url, {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({
        jsonrpc: "2.0",
        method: "getTokenAccounts",
        id: "helius-test",
        params: {
          page: page,
          limit: 1000,
          displayOptions: {},
					//mint address for the token we are interested in
          mint: "CKfatsPMUf8SkiURsDXs7eK6GWb4Jsd6UDbs7twMCWxo",
        },
      }),
    });

		// Check if any error in the response
      if (!response.ok) {
        console.log(
          `Error: ${response.status}, ${response.statusText}`
        );
        break;
      }

    const data = await response.json();
  	// Pagination logic. 
    if (!data.result || data.result.token_accounts.length === 0) {
      console.log(`No more results. Total pages: ${page - 1}`);
      break;
    }
    console.log(`Processing results from page ${page}`);
 		// Adding unique owners to a list of token owners. 
    data.result.token_accounts.forEach((account) =>
      allOwners.add(account.owner)
    );
    page++;
  }

  fs.writeFileSync(
    "output.json",
    JSON.stringify(Array.from(allOwners), null, 2)
  );
};


```

在上面的示例中，在分页浏览所有代币账户时，多次调用getTokenAccounts方法。API 响应将为每个代币账户提供以下数据：

“地址”：“CVMR1nbxTcQ7Jpa1p137t5TyKFii3Y7Vazt9fFct3tk9”，

“薄荷”：“SHDWyBxihqiCj6YekG2GUr7wqKLeLAMK1gHZck9pL6y”，

“所有者”：“CckxW6C1CjsxYcXSiDbk7NYfPLhfqAm3kSB5LEZunnSE”，

“金额”：100000000，

“委托金额”：0，

“冻结”：错误

}，

我们从这些代币账户中提取了所有者，并将其添加到我们的列表中。如果我们愿意，我们还可以存储每个代币账户持有的代币数量，以找出最大的持有者。

一旦完成，我们需要做的就是调用该方法：

```
findHolders();
```

我们的getTokenHolders.js文件中的完整代码应如下所示：

```
const url = `https://mainnet.helius-rpc.com/?api-key=`;
const fs = require("fs");


const findHolders = async () => {
  let page = 1;
  let allOwners = new Set();

  while (true) {
    const response = await fetch(url, {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({
        jsonrpc: "2.0",
        method: "getTokenAccounts",
        id: "helius-test",
        params: {
          page: page,
          limit: 1000,
          displayOptions: {},
          mint: "DezXAZ8z7PnrnRJjz3wXBoRgixCa6xjnB7YaB1pPB263",
        },
      }),
    });

		// Check if any error in the response
      if (!response.ok) {
        console.log(
          `Error: ${response.status}, ${response.statusText}`
        );
        break;
      }

    const data = await response.json();

    if (!data.result || data.result.token_accounts.length === 0) {
      console.log(`No more results. Total pages: ${page - 1}`);

      break;
    }
    console.log(`Processing results from page ${page}`);
    data.result.token_accounts.forEach((account) =>
      allOwners.add(account.owner)
    );
    page++;
  }

  fs.writeFileSync(
    "output.json",
    JSON.stringify(Array.from(allOwners), null, 2)
  );
};

findHolders();

```

## 输出

我们的代码的输出将是所有持有者的列表，看起来类似于：

\[

“111An9SVxuPpgjnuXW9Ub7hcVmZpYNrYZF4edsGwJEW”，

“11Mmng3DoMsq2Roq8LBcqdz6d4kw9oSD8oka9Pwfbj”，

“112uNfcC8iwX9P2TkRdJKyPatg6a4GNcr9NC5mTc2z3”，

“113uswn5HNgEfBUKfK4gVBmd2GpZYbxd1N6h1uUWReg”，

“11CyvpdYTqFmCVWbJJeKFNX8F8RSjNSYW5VVUi8eX4P”，

“11MANeaiHEy9S9pRQNu3nqKa2gpajzX2wrRJqWrf8dQ”，

…

]

## 结论

在本指南的最后，我们成功介绍了通过 Helius getTokenAccounts API识别 Solana 代币持有者的过程。

如有不明白或者不清楚的地方，请加入官方电报群：[**https://t.me/gtokentool**](https://t.me/gtokentool)
