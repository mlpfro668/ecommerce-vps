# 搬瓦工 Ecommerce VPS：CN2 GIA 电商套餐全配置价格对比，附 SLA 新款与机房迁移选购指南

在搬瓦工的官网上，"Ecommerce VPS" 不是一个单独的按钮，而是一整条产品线：从季付 49.99 美元的 CN2 GIA-E 入门款，到月付一千多美元、带 99.99% SLA 保障的高端货，都归在 E-Commerce 名下。很多人搜这个词时其实是想知道三件事：它和普通 KVM 套餐差在哪、到底值不值差价、以及现在有哪些配置和价格可买。这篇文章把官网当前在售的全部套餐整理成表，再说说选购时真正需要权衡的几个点。

## Ecommerce VPS 在搬瓦工官网里指什么

搬瓦工（BandwagonHost，运营方是 IT7 Networks Inc.）目前在售的套餐分三大类：Basic VPS（普通 KVM）、E-Commerce（电商优化）和 Ultra（香港、大阪、东京等高端机房）。E-Commerce 是中间的主力线，官方给它的定位是提供"更好的连通性，包括对中国大陆的优质线路"。

这条线下现在有三个子系列：

- **CN2 GIA-E 经典款**：洛杉矶中国电信 CN2 GIA 线路起步，2.5Gbps 带宽起，可在 10 个以上 E-Commerce 级机房之间免费自动迁移，这是最经典、讨论度最高的一档。
- **ECOMMERCE SLA 洛杉矶**：新款，走洛杉矶 DC5 SLA 机房，用 AMD 专用核心、ECC 内存和本地 NVMe 硬盘，承诺 99.99% 在线率，配置上明显更"企业向"。
- **迪拜 ECOMMERCE**：面向中东市场，1Gbps 带宽，价格反而比同配 CN2 GIA-E 便宜，但不支持 IPv6。

三个子系列都是 KVM 虚拟化，跑在自研的 KiwiVM 面板上，支持 CentOS、Debian、Ubuntu、Rocky Linux、AlmaLinux，每台机器带 1 个独立 IPv4 和一个 /64 的 IPv6 子网（迪拜款除外），root 权限完整开放。

## 三条产品线分别适合谁

CN2 GIA-E 是大多数人的默认答案。它解决的核心问题是电信去程走 CN2 GIA，同时给联通提供 2.5Gbps 的电信级传输通道，其余目的地走电商优化网络，官方页面还写明与 Google 有直连对等。对做外贸站、面向国内用户的应用来说，这条线是搬瓦工全部套餐里讨论度最高的。

SLA 款解决的是另一个问题：稳定性承诺和故障处理。标准套餐的在线率保障是 99.95%，SLA 款直接提到 99.99%，并写明机房达到 Tier III 标准，有 SOC 1 Type 2、SOC 2 Type 2、ISO 27001、PCI DSS 等一串认证。如果你跑的是不能随便宕机的业务，这部分差价买的就是合同层面的保障。

迪拜款是个特殊定位。同样 20GB 硬盘、1GB 内存的配置，迪拜只要 19.99 美元/月，比 CN2 GIA-E 还便宜，但流量只有一半（500GB/月），带宽降到 1Gbps，也没有 IPv6。目标客户很明确：业务在中东、对国内线路没要求的用户。

## 搬瓦工 Ecommerce VPS 全套餐配置与价格总表

以下是官网当前展示的全部在售套餐（币种均为美元），价格按月付 / 季付 / 半年付 / 年付列出，横线表示官方未提供该计费周期。

**CN2 GIA ECOMMERCE 经典款（10+ 机房可自由迁移）**

| 套餐 | 配置（内存/CPU/硬盘） | 流量/带宽 | 月付 | 季付 | 半年付 | 年付 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 20G CN2 GIA-E | 1GB / 2核 / 20GB | 1TB / 2.5Gbps | — | $49.99 | $89.99 | $169.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=87) |
| 40G CN2 GIA-E | 2GB / 3核 / 40GB | 2TB / 2.5Gbps | — | $89.99 | $169.99 | $299.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=88) |
| 80G CN2 GIA-E | 4GB / 4核 / 80GB | 3TB / 2.5Gbps | $56.99 | $149.99 | $289.99 | $549.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=89) |
| 160G CN2 GIA-E | 8GB / 6核 / 160GB | 5TB / 5Gbps | $86.99 | $239.99 | $459.99 | $879.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=90) |
| 320G CN2 GIA-E | 16GB / 8核 / 320GB | 8TB / 5Gbps | $159.99 | $459.99 | $869.99 | $1599.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=91) |
| 640G CN2 GIA-E | 32GB / 10核 / 640GB | 10TB / 10Gbps | $289.99 | $799.99 | $1499.99 | $2759.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=92) |
| 1280G CN2 GIA-E | 64GB / 12核 / 1280GB | 12TB / 10Gbps | $549.99 | $1559.99 | $2979.99 | $5499.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=93) |
| 1280G 大流量 15T | 64GB / 12核 / 1280GB | 15TB / 10Gbps | $679.00 | $1935.00 | $3670.00 | $6790.00 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=160) |
| 1280G 大流量 20T | 64GB / 12核 / 1280GB | 20TB / 10Gbps | $899.00 | $2562.00 | $4860.00 | $8999.00 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=161) |

**ECOMMERCE SLA 洛杉矶（99.99% SLA，DC5 机房）**

| 套餐 | 配置（内存/CPU/硬盘） | 流量/带宽 | 月付 | 季付 | 半年付 | 年付 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 20G SLA | 1GB ECC / 2核 AMD / 20GB NVMe | 1TB / 2.5Gbps | — | $65.89 | $125.99 | $239.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=164) |
| 40G SLA | 2GB ECC / 3核 AMD / 40GB NVMe | 2TB / 2.5Gbps | — | $116.99 | $219.99 | $399.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=165) |
| 80G SLA | 4GB ECC / 4核 AMD / 80GB NVMe | 3TB / 2.5Gbps | $69.99 | $199.99 | $379.99 | $699.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=166) |
| 160G SLA | 8GB ECC / 6核 AMD / 160GB NVMe | 5TB / 5Gbps | $109.99 | $299.99 | $569.99 | $1099.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=167) |
| 320G SLA | 16GB ECC / 8核 AMD / 320GB NVMe | 8TB / 5Gbps | $199.99 | $569.99 | $1079.99 | $1999.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=168) |
| 640G SLA | 32GB ECC / 10核 AMD / 640GB NVMe | 10TB / 10Gbps | $369.99 | $1055.99 | $1999.99 | $3699.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=169) |
| 1280G SLA | 64GB ECC / 12核 AMD / 1280GB NVMe | 12TB / 10Gbps | $699.99 | $1989.99 | $3779.99 | $6999.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=170) |
| 1280G SLA 大流量 15T | 64GB / 12核 / 1280GB NVMe | 15TB / 10Gbps | $879.99 | $2509.99 | $4768.99 | $8799.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=171) |
| 1280G SLA 大流量 20T | 64GB / 12核 / 1280GB NVMe | 20TB / 10Gbps | $1159.99 | $3299.99 | $6269.99 | $11598.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=172) |

**迪拜 ECOMMERCE（中东方向，1Gbps，无 IPv6）**

| 套餐 | 配置（内存/CPU/硬盘） | 流量/带宽 | 月付 | 季付 | 半年付 | 年付 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 20G 迪拜 | 1GB / 2核 / 20GB | 500GB / 1Gbps | $19.99 | $49.99 | $89.99 | $169.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=114) |
| 40G 迪拜 | 2GB / 3核 / 40GB | 1TB / 1Gbps | $32.99 | $89.99 | $169.99 | $299.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=115) |
| 80G 迪拜 | 4GB / 4核 / 80GB | 2TB / 1Gbps | $56.99 | $149.99 | $289.99 | $549.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=116) |
| 160G 迪拜 | 8GB / 6核 / 160GB | 3TB / 1Gbps | $86.99 | $239.99 | $459.99 | $879.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=117) |
| 320G 迪拜 | 16GB / 8核 / 320GB | 4TB / 1Gbps | $159.99 | $459.99 | $869.99 | $1599.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=118) |
| 640G 迪拜 | 32GB / 10核 / 640GB | 5TB / 1Gbps | $289.99 | $799.99 | $1499.99 | $2759.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=119) |
| 1280G 迪拜 | 64GB / 12核 / 1280GB | 6TB / 1Gbps | $549.99 | $1559.99 | $2979.99 | $5399.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=120) |

**同页在售的 Basic KVM（普通入门款）**

| 套餐 | 配置（内存/CPU/硬盘） | 流量/带宽 | 月付 | 季付 | 半年付 | 年付 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 20G KVM | 1GB / 2核 / 20GB | 1TB / 1Gbps | — | — | — | $49.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=44) |
| 40G KVM | 2GB / 3核 / 40GB | 2TB / 1Gbps | — | — | $52.99 | $99.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=45) |
| 80G KVM | 4GB / 4核 / 80GB | 3TB / 1Gbps | $19.99 | $59.99 | $107.99 | $199.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=46) |
| 160G KVM | 8GB / 5核 / 160GB | 4TB / 1Gbps | $39.99 | $112.99 | $213.99 | $399.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=47) |
| 320G KVM | 16GB / 6核 / 320GB | 5TB / 1Gbps | $79.99 | $227.99 | $432.99 | $799.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=48) |
| 480G KVM | 24GB / 7核 / 480GB | 6TB / 1Gbps | $119.99 | $341.99 | $649.49 | $1199.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=49) |

**Ultra 高端机房款（新加坡 / 大阪 / 香港 / 东京，季付和半年付同样可选）**

| 套餐 | 配置（内存/CPU/硬盘） | 流量/带宽 | 月付 | 年付 | 购买 |
| --- | --- | --- | --- | --- | --- |
| 新加坡 40G | 2GB / 2核 / 40GB | 500GB / 1.5Gbps | $49.99 | $499.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=173) |
| 新加坡 80G | 4GB / 4核 / 80GB | 1TB / 1.5Gbps | $86.99 | $869.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=174) |
| 新加坡 160G | 8GB / 6核 / 160GB | 2TB / 2.5Gbps | $165.99 | $1665.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=175) |
| 新加坡 320G | 16GB / 8核 / 320GB | 4TB / 2.5Gbps | $329.99 | $3199.00 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=176) |
| 新加坡 640G | 32GB / 10核 / 640GB | 6TB / 5Gbps | $549.99 | $5549.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=177) |
| 新加坡 1280G | 64GB / 12核 / 1280GB | 8TB / 5Gbps | $1059.99 | $10559.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=178) |
| 大阪 40G | 2GB / 2核 / 40GB | 500GB / 1.5Gbps | $49.99 | $499.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=134) |
| 大阪 80G | 4GB / 4核 / 80GB | 1TB / 1.5Gbps | $86.99 | $869.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=135) |
| 大阪 160G | 8GB / 6核 / 160GB | 2TB / 1.5Gbps | $165.99 | $1665.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=136) |
| 大阪 320G | 16GB / 8核 / 320GB | 4TB / 1.5Gbps | $329.99 | $3199.00 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=137) |
| 大阪 640G | 32GB / 10核 / 640GB | 6TB / 1.5Gbps | $549.99 | $5549.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=138) |
| 大阪 1280G | 64GB / 12核 / 1280GB | 8TB / 1.5Gbps | $1059.99 | $10559.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=139) |
| 香港 40G | 2GB / 2核 / 40GB | 500GB / 1Gbps | $89.99 | $899.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=95) |
| 香港 80G | 4GB / 4核 / 80GB | 1TB / 1Gbps | $155.99 | $1559.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=96) |
| 香港 160G | 8GB / 6核 / 160GB | 2TB / 1Gbps | $299.99 | $2999.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=97) |
| 香港 320G | 16GB / 8核 / 320GB | 4TB / 1Gbps | $589.99 | $5899.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=98) |
| 香港 640G | 32GB / 10核 / 640GB | 6TB / 1Gbps | $989.99 | $9989.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=122) |
| 香港 1280G | 64GB / 12核 / 1280GB | 8TB / 1Gbps | $1889.99 | $18989.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=124) |
| 东京 40G | 2GB / 2核 / 40GB | 500GB / 1.2Gbps | $89.99 | $899.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=108) |
| 东京 80G | 4GB / 4核 / 80GB | 1TB / 1.2Gbps | $155.99 | $1559.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=109) |
| 东京 160G | 8GB / 6核 / 160GB | 2TB / 1.2Gbps | $299.99 | $2999.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=110) |
| 东京 320G | 16GB / 8核 / 320GB | 4TB / 1.2Gbps | $589.99 | $5899.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=111) |
| 东京 640G | 32GB / 10核 / 640GB | 6TB / 1.2Gbps | $989.99 | $9989.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=123) |
| 东京 1280G | 64GB / 12核 / 1280GB | 8TB / 1.2Gbps | $1889.99 | $18989.99 | [ 购买](https://bandwagonhost.com/aff.php?aff=79616&pid=125) |

所有套餐都不提供managed托管服务，属于纯自助型 VPS。想看实时库存和更多在售方案，可以从 [👉 搬瓦工全部套餐列表](https://bit.ly/BandwagonHost) 进入官网核对。

## CN2 GIA-E：为什么它是卖得最多的 Ecommerce 套餐

CN2 GIA-E 的核心卖点集中在两条：线路和迁移自由度。洛杉矶机房走中国电信 CN2 GIA，去程直连；联通方向由电信提供 2.5Gbps 企业级传输；其他目的地走电商优化的优质网络，并且和 Google 直连对等。日本方向则走大阪 Equinix 机房的 Softbank 2.5Gbps 中转。

迁移自由度是它区别于 Basic 套餐的关键。官方套餐页写明"本套餐提供 10 个以上 E-Commerce 级机房，可在数据中心之间免费自动迁移"。按第三方实测整理，这个列表实际覆盖 12 个以上机房，包括洛杉矶 DC6（CN2 GIA-E）和 DC9（CN2 GIA）、日本、荷兰等地。买了 20G 款之后在 KiwiVM 后台点一下就能换机房，流量配额不变，试错成本几乎为零。

计费周期上也留了余地：20G 款只有季付（$49.99）和年付（$169.99）两档，80G 以上才开放月付。年付折算下来比季付续费要省——20G 款季付一年下来是 $199.99，年付直接是 $169.99。

要买的话，最低门槛是 [👉 20G CN2 GIA-E 季付套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=87)；需要 2GB 内存跑稍重的应用，[👉 40G 款](https://bandwagonhost.com/aff.php?aff=79616&pid=88) 季付 $89.99 是同系列里的常见选择。

## SLA 套餐多花的钱买到了什么

拿最小配置对比：20G CN2 GIA-E 季付 $49.99，20G SLA 季付 $65.89，一季差 $15.9。这 $15.9 换来的东西在官方套餐页写得比较具体：

- **99.99% SLA 在线率承诺**，标准款是 99.95%；
- **硬件规格升级**：AMD 专用核心、ECC 内存、本地 NVMe RAID-10 硬盘，而不是普通款的 Intel Xeon 共享配置；
- **每两周免费更换一次 IP**，标准款换 IP 是付费的；
- 机房层面：Tier III 认证机房、双路供电加柴油发电机、双网卡双光纤路径、24/7 NOC 监控，并且与 Apple、Google、Facebook、字节跳动等网络直连对等。

线路本身两边的方向一致：电信 CN2 GIA/CTGNet、联通 Premium（AS10099）、移动 CMIN2（AS58807）三网优化都在。

关于宕机补偿，多个第三方整理提到 SLA 套餐故障时可按预付时长获得补偿，严重故障最高补偿一个月的使用时长，补偿形式是给机器延长时长而不是退现金。这一条建议下单前在官方 Service Level Agreement 页面再确认一次细节。

适合买 SLA 的人群很窄但很明确：外贸电商站、付费业务 API 这类宕机一小时就心疼钱的应用。个人博客和代理用途，99.95% 的标准款其实够用。

## Ecommerce 套餐和 Basic、Ultra 怎么选

同配置直接比一下最直观。20G Basic KVM 年付 $49.99，20G CN2 GIA-E 年付 $169.99，差了三倍多。配置几乎一样（1GB 内存、2 核、20GB SSD、1TB 流量），差的部分全在网络：Basic 是 1Gbps 普通线路，机房只有少数几个可选；GIA-E 是 2.5Gbps 三网优化线路加 10+ 机房随便迁。

所以判断标准其实就一个：你的用户在哪。用户在国内或亚太，对延迟敏感，GIA-E 的差价是花在刀刃上的；只是挂个海外业务、不面向国内用户，Basic 年付 $49.99 是全网少见的低价位，没必要多花。

Ultra 系列则是另一个量级。香港、东京、大阪机房的延迟比洛杉矶低得多，但流量给得也小气：最低配 40G 只有 500GB/月，价格却是 $49.99/月（大阪）到 $89.99/月（香港、东京）。月流量需求超过 1TB 的，基本只能回洛杉矶方向找答案。

一个折中思路：先买 GIA-E 入门款，用一段时间如果发现速度不够再评估要不要升 Ultra。反正机房迁移免费，损失的只有可能的价格差。

## cPanel、流量和几个容易踩的坑

**cPanel 授权要另买。** Ecommerce 套餐本身不带 cPanel/WHM 授权，这是独立商业软件，需要单独购买 External VPS 类型的授权。有第三方教程算过账：cPanel/WHM 实际跑起来建议 2GB 内存起步，也就是说 40G 以上配置才比较从容；1GB 内存的 20G 款装 cPanel 会很勉强，轻量建站用宝塔面板这类免费方案更现实。

**流量按双向计费。** 有第三方整理指出搬瓦工的流量统计是进站加出站双向计算，实际可用流量比标称数字看起来要少，规划大流量业务时要按这个口径估算。

**超流量的后果是停机而不是扣费。** 官方知识库写得很清楚：流量用完后不会产生任何超额费用，VPS 会被自动暂停直到当前计费周期结束。想提前恢复只能升级套餐，流量会在下一个计费周期重置。这一点比那些超 1GB 罚一笔的商家友好，但做电商的要知道自己的业务在暂停期间是裸奔状态。

**快照和备份免费。** 所有套餐都在 KiwiVM 面板里内置免费自动备份和免费快照，快照可以导入导出，也能拿来跨机房迁移数据。这个功能不少商家要单独收费。

## 优惠码现状：别指望太多

截至 2026 年 9 月前后，多个搬瓦工资讯站的整理口径一致：官网目前没有长期有效的公开优惠码。历史上流传的循环折扣码（力度大约 6.6% 到 6.8%）均已过期，比如老牌的 BWHCGLUKKB 已经失效，2026 年初短暂出现过的 NODESEEK2026 也只活了两天。搬瓦工近年更常见的优惠方式是限量套餐补货和限时活动，而不是可复用的优惠码。下单前可以在结算页看一眼有没有可用促销，但别按着某个旧码等。

## 购买流程和上手要做的几件事

购买流程不复杂：选套餐 → 注册账号（邮箱）→ 付款 → 进入 KiwiVM 面板。付款后 VPS 是即时开通的，不需要等人工审核。

拿到机器后建议按这个顺序操作：

1. 在 KiwiVM 里装系统，官方支持 CentOS、Debian、Ubuntu、Rocky Linux、AlmaLinux，也支持手动挂 ISO 安装；
2. 做一次初始快照，系统配好环境后再拍一次，免费的不用白不用；
3. 设置 rDNS（PTR 记录），发邮件类业务需要提前配好；
4. 记住流量重置日，在面板的用量统计里盯一下消耗速度。

机房的默认位置在购买时选择，后续随时可以在面板里迁移，这也是很多人选 GIA-E 而不是 Basic 的隐性理由之一。准备好了可以直接从 [👉 搬瓦工 E-Commerce 套餐购买入口](https://bit.ly/BandwagonHost) 进官网下单。

## 最后的选择建议

把话说短：面向国内用户、预算有限，选 20G 或 40G CN2 GIA-E，季付起步；业务不能宕机、愿意为 SLA 付费，直接上 ECOMMERCE SLA 洛杉矶系列，40G 起步比较稳；用户在中东，看迪拜款；纯海外业务图便宜，Basic KVM 年付款就够。搬瓦工的套餐体系复杂，但好在迁移免费、快照免费，选错了的纠正成本不算高——真正贵的只有月流量超配和 SLA 档位的差价，下单前把自己的流量账算清楚就行。
