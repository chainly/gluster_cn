# # # 入门

本教程将涵盖不同的选项，用于获取 Gluster
群集启动和运行。这里是一个破败的我们需要做的步骤。


若要开始，我们将复习一些普通的东西，你需要知道的
设置 Gluster。

接下来，选择您想要使用来设置您的第一个簇的方法︰
-虚拟机中
-到裸露的金属服务器
-对亚马逊的 EC2 实例

最后，我们将安装 Gluster，创建几个卷，并使用测试
他们。

# # # 常见的安装标准

无论在哪里，你将安装 Gluster，它有助于我们理解
是什么运动部件上的一些关键概念。

首先，它是重要的是理解 GlusterFS 不是真正
文件系统本身。它将连接到现有的文件系统

一个 （或多个） 的大块，所以该数据被写入或读出来的
Gluster 同时获取分布在多个主机。这

意味着你可以使用来自任何主机空间可用。
通常情况下，XFS 建议，但可以用其他文件系统
以及。EXT4 最常用于当 XFS 不是，但你可以 （和

许多人做） 使用适合你的另一个文件系统。现在，我们

明白了，我们可以定义一些使用中的常用术语
Gluster。

-A * * 信任池 * * 指的是集体中的主机给定
Gluster 群集。
-A * * 节点 * * 或"服务器"是指任何服务器的一部分
受信任的游泳池。一般情况下，这假设所有的节点都在同一

受信任的游泳池。
-A * * 砖 * * 用来指任何设备 （真的这意味着
文件系统），用于 Gluster 存储。
-* * 出口 * * 是指 brick(s) 的安装路径对给定
服务器，例如，brick1/出口 /
一词 * * 全球 Namespace * * 是推脱说 Gluster
卷
-A * * Gluster 卷 * * 是一家集的一个或多个砖 （
当然，这通常是两个或更多）。这是到委实

/ 等/出口 NFS 的条目。
-* * 金纳米花 * * 和 * * kNFS * *。金纳米花是如何我们提到我们的内联 NFS

服务器。kNFS 代表内核 NFS，或者，像大多数人会说，

只是普通的 NFS。大多数情况下，你会想要禁用上的 kNFS 服务

Gluster 节点。Gluster NFS 不需要任何额外的

配置和你一样的作品会预料 nfsv3 时。它是

可以配置 NFS Gluster，如果你想要生活在和谐
自。

其他注意事项︰

-对于此测试，如果你没有 DNS 设置，你可以侥幸
为两个节点使用 /etc/hosts 条目。但是，当您移动

从这个基本设置到使用 Gluster 在生产中，正确的 DNS
条目 （正向和反向） 和 NTP 是必不可少的。
-在安装操作系统时，不格式化 Gluster
存储磁盘 ！我们将使用 mkfs 命令的特定设置

后来当我们设置 Gluster。如果您要测试跟单

磁盘 （不推荐），请确保创业自由分区或
两个，以便您可以设置格式或重新格式化后，使用由 Gluster
随意在您的测试。
-防火墙是伟大的除了当他们不是。对于存储服务器，

能够在没有防火墙可以受信任环境中运行
意味着巨额收益的性能，和建议。在种情况下你绝对

需要设置防火墙，看一看
[客户端设置](../ 管理员指南设置 Clients.md) 为

使用的端口的信息。

点击这里 [获取 started](./Quick_start.md)
