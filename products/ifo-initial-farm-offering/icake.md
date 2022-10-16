---
description: CAKE定期质押和IFO分配
---

# iCAKE

### 什么是 iCAKE？

iCAKE 类似于之前 IFO CAKE质押池中的"IFO 积分“，该池在 主厨合约v2 迁移期间中停用。此次更新后，iCAKE 决定了PancakSwap IFO公开发售中每个地址能提交的 CAKE 数量上限。举个例子，如果您的 iCAKE 数值为 200，您可以在即将到来的 IFO 公开销售中提交最高 200 个 CAKE 代币。

**iCAKE 不是一个新的代币，他是PancakeSwap IFO系统中使用的一个数值度量。**

### iCAKE 怎么计算的？

您拥有的 iCAKE 数量是根据您在 CAKE 定期质押池中质押的 CAKE 数量和您当前定期质押仓位的总质押时长确定的。

&#x20;iCAKE 的计算方式基于所有 iCAKE 用户的质押持续时间阈值。&#x20;

如果您的质押时长超过阈值，则您拥有的 iCAKE 数量等于您质押的 CAKE 数量。&#x20;

如果您的质押时长低于阈值，您拥有的 iCAKE 数量将线性减少和调整。&#x20;

如果您的质押期结束，那么您的iCAKE数量将为0。

举例说明，如果阈值为20周：

* 您当前的定期质押锁定时间为 25 周并且质押 200 个CAKE。 那么您拥有的 iCAKE 数量是 200。&#x20;
* 您当前的定期质押锁定时间为 10 周并且质押 200 个 CAKE。 那么您拥有的 iCAKE 数量等于 200 × (10 ÷ 20) = 100。&#x20;
* 您当前的定期质押锁定时间为 2 周并且质押 200 个 CAKE。 那么你拥有的 iCAKE 数量等于 200 × (2 ÷ 20) = 20。&#x20;
* 您定期质押锁定时间为 2 周并且质押 200 个CAKE。 但是您的质押已经结束到期， 那么您拥有的 iCAKE 数量为 0。

| 情况分类    | 您的定期质押锁仓时长等于或者长于阈值 | 您的定期质押锁仓时长短于阈值                |
| ------- | ------------------ | ----------------------------- |
| iCAKE数量 | 等于您的锁仓CAKE数量       | 等于您的锁定 CAKE 数量 x（您的质押持续时长/阈值） |

### 如何查看我拥有多少个 iCAKE?

<figure><img src="../../.gitbook/assets/image3.png" alt=""><figcaption></figcaption></figure>

您可以在[IFO界面](https://pancakeswap.finance/ifo)看到您拥有的iCAKE数量。

### 如何增加我拥有的iCAKE数量?

您可以增加iCAKE数量的途径有：

* 在CAKE定期锁仓糖浆池中增加您质押的CAKE数量
* 延长您的锁仓时间（如果您目前的总锁仓时间短于当前的阈值）

<figure><img src="../../.gitbook/assets/image2.png" alt=""><figcaption></figcaption></figure>

您可以在调整或初始化锁仓数量或时间时预览产生的 iCAKE 数量。

### iCAKE 计算的阈值是多少？

在每两个IFO之间，厨房会根据**定期质押CAKE糖浆池的平均质押时长**来优化**阈值**。调整将会在**所有社交媒体渠道**上公布。

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>图片仅供参考，实际「阈值」周数可于当期IFO界面查看。</p></figcaption></figure>

您可以通过悬停或点击蛋糕糖浆池窗口中带下划线的 iCAKE 文本，来查看当前**阈值**。
