# 多签钱包创建教程

## 什么是多签钱包： <a href="#shen-me-shi-duo-qian-qian-bao" id="shen-me-shi-duo-qian-qian-bao"></a>

与多签钱包对应的是单签钱包，我们要往区块链上发送一笔转账操作，需要用钱包生成一个签名，我们自己签好名把交易发送出去，这就是典型的单签钱包，也是我们平时常用的钱包。

多签钱包，顾名思义，就是需要多个人去签名执行某个操作的钱包。使用多签钱包进行转账，往往需要 >= 1 个人去签名发送交易，转账操作才可以完成。使用多签钱包时，我们可以指定 m/n 的签名模式，就是 n 个人里面有 m 个人签名即可完成操作。比如 2/3 签名模式，就是 3 个人里面有两个人签名就可以。

ETH/ERC20 (包括 BSC/BEP20 等EVM链）的多签采用轻量智能合约（smart contract）方式。

## **适用场景：**

1\. 用于需要多人管理资产，避免资产被个人挪用；

2\. 通过多签对资产进行多地址签名管理，增强资产安全性；

3.其他安全应用场景。

## 多签钱包创建： <a href="#duo-qian-qian-bao-chuang-jian" id="duo-qian-qian-bao-chuang-jian"></a>

1、打开TokenPocket，首次使用点击【我没有钱包】，选择【多签钱包】进行创建。已经使用TokenPocket创建或导入过的用户也可以打开钱包后点击右上角第一个图标，添加多签钱包。

![](https://help.tokenpocket.pro/~gitbook/image?url=https%3A%2F%2F261497644-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F-MMF2k4MCaxErpZyah2d%252Fuploads%252FZrnFkTeeiVZIWkIqp46v%252Fimage.png%3Falt%3Dmedia%26token%3D497787db-cdcf-480f-9c2a-ab8c8e904228\&width=768\&dpr=4\&quality=100\&sign=60753d22\&sv=2)

2、在多签网络中选择需要创建多签的网络，例如这里选择币安智能链，请认真阅读【多签创建流程】中的提示内容，阅读完成后点击下一步。

![](https://help.tokenpocket.pro/~gitbook/image?url=https%3A%2F%2F261497644-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F-MMF2k4MCaxErpZyah2d%252Fuploads%252F9SfzlCBOMAFOvFx8KW2F%252F2%2520%25E6%258B%25B7%25E8%25B4%259D.png%3Falt%3Dmedia%26token%3Ded5c1126-cf63-400f-a39c-06af87eb69c7\&width=768\&dpr=4\&quality=100\&sign=a003a8c0\&sv=2)

3、多签钱包创建的步骤是最核心的内容，下图中将每一个类型的内容进行了展示，内容如下:

【多签钱包名】和日常创建钱包名一样，可以自定义设置，并不会上链。

【设置管理钱包】设置多签钱包的管理钱包，多签钱包由管理钱包共同进行管理和控制，最多支持30个管理钱包设置。管理钱包可以灵活设置，适用于企业或团队资产管理或个人的多元化使用。

【最少确认签名数】设置钱包最低签名数，当满足最低签名数时，即可发起转账、合约交互等链上操作。最小确认签名数建议设置大于2以上的数值，可以兼顾安全与便捷。

【费用信息】该费用属于在链上执行多签钱包创建的网络费用，TokenPocket不会收取任何费用。

【支付钱包】这里可以点击选择钱包中导入的钱包地址进行创建Gas（矿工费）费用的支付。

当一切设置妥当后，点击【确认】即可看到多签钱包创建中的提示，界面中可以点击跳转到BSC区块链浏览器上查看相关创建信息。

![](https://help.tokenpocket.pro/~gitbook/image?url=https%3A%2F%2F261497644-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F-MMF2k4MCaxErpZyah2d%252Fuploads%252F6LYCpsVCIcnxl8OG972J%252Fimage.png%3Falt%3Dmedia%26token%3D9e6568f2-e9c6-48ae-9fd1-71af6be2c03e\&width=768\&dpr=4\&quality=100\&sign=59ce1c5b\&sv=2)

4、耐心等待合约部署成功后就完成了多签钱包的创建。点击钱包左上角菜单，在钱包列表中可以非常直观的分辨出多签钱包和单签钱包的区别，在钱包切换中会更加的方便。

![](https://help.tokenpocket.pro/~gitbook/image?url=https%3A%2F%2F261497644-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F-MMF2k4MCaxErpZyah2d%252Fuploads%252Fs0fqIgkrq4KDDStxsgZg%252F4%2520%25E6%258B%25B7%25E8%25B4%259D.png%3Falt%3Dmedia%26token%3Dd377d387-be1c-4018-bdb2-bfa48105ad53\&width=768\&dpr=4\&quality=100\&sign=c270db8a\&sv=2)

5、多签钱包创建成功后，点击蓝色区域右上角【详情】在这里可以查看详情信息，主要有【多签队列】和【多签管理】两个分类。

![](https://help.tokenpocket.pro/~gitbook/image?url=https%3A%2F%2F261497644-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F-MMF2k4MCaxErpZyah2d%252Fuploads%252FPtfm6oRddkGpwlZtjSD3%252F5%2520%25E6%258B%25B7%25E8%25B4%259D.png%3Falt%3Dmedia%26token%3Dbbaeede9-aa1e-421e-a849-e159241b26a1\&width=768\&dpr=4\&quality=100\&sign=f9e067f2\&sv=2)

6、多签队列中会显示生成的多签订单，可以点击并完成订单；多签管理中可以查看【最小确认签名数】、【链上最新Nonce】和【关联钱包】等信息，其中关联钱包就是管理地址，如果有未导入的地址，可以通过点击【导入该钱包】使用私钥或助记词导入，关联钱包的是否导入会影响后续的转账或DApp的使用的调用方式。

![](https://help.tokenpocket.pro/~gitbook/image?url=https%3A%2F%2F261497644-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F-MMF2k4MCaxErpZyah2d%252Fuploads%252FL2DVEx0uHaMxzsMpUN7g%252Fimage.png%3Falt%3Dmedia%26token%3Dd8e41b55-4bf5-4d3d-bd11-66def7b97745\&width=768\&dpr=4\&quality=100\&sign=64e31881\&sv=2)

总结一下，EVM链上的多签钱包就是一个智能合约，创建多签钱包不需要备份助记词或私钥、不需要设置密码、不需要复杂的代码。创建多签钱包的重点是【管理钱包】和【最小确认签名数】的合理设置，只有经过合理的设置才能发挥多签钱包最大程度的安全和便捷。一般常用的多签有 2/3 、3/5等方式， 需根据个人情况进行选择。

如有不明白或者不清楚的地方，请加入官方电报群：[**https://t.me/gtokentool**](https://t.me/gtokentool)
