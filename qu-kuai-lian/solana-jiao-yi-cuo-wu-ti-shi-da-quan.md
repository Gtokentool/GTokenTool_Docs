---
description: 本文记录一些Sol链的常见错误及原因
---

# Solana交易错误提示大全

**1.交易代币时错误提示"Program Error. "instruction #3 Failed- Account is frozen"是什么意思?**

答: 代币账户被冻结，未放弃权限的代币的管理者Owner，可以冻结代币下的账户，被冻结的账户无法进行交易、转账等操作。

**2.错误提示: "Program Error: "Instruction #5 Failed - null"" 或 "Program Error: "Instruction #5 Failed - InvalidInput""**

答: 交易项的#5出现错误，一般是交易参数错误导致。 这里的#几代表哪条交易信息出错。

**3.错误提示: "Program Error: "Instruction #3 Failed - insufficient funds""**

答: 交易所需资金不足提示。
