### 刷机步骤

#### 刷机准备

- 建议下载好固件后，对固件的md5/sha1校验码进行核对，以保证固件完整性；
- 建议刷机全程使用电脑端谷歌Chrome，或者Chromium内核的浏览器进行操作；

#### 刷机术语

> 为消除小白在刷机过程中的疑惑，下面列出一下华硕/梅林固件刷机的基本术语及我自己的解释，希望对大家有所帮助。如果你对下面的内容已经比较清楚，那么可以跳过这部分直接进入到刷机流程。

1. **固件双清**：双清就是要清除：1. nvram配置，2：JFFS分区文件。固件的很多设置都是储存在nvram中，例如拨号方式、拨号上网帐号密码、无线网络设置等；固件的很多文件是储存在JFFS分区的，例如流量分析储存的流量数据，SSL证书，UU加速器程序等。一般同类型固件互刷不需要进行双清，不同类型固件互刷视情况要进行双清，以保证路由器刷机后处于最佳工作状态。

   > **如何双清路由器**：进入【系统管理 】–【 恢复/导出/上传设置】，勾选恢复按钮旁的选择框，然后点击恢复按钮。

2. **恢复出厂**：恢复出厂就是清除固件的nvram配置，但是不清除JFFS分区文件。这样流量分析、SSL证书等文件并不会丢失。值得注意的是很多朋友有用【导出设置】来备份固件配置的习惯，而在刷固件，特别是不同类型固件互刷的情况下，是不适用使用备份的配置来恢复刚刚进行了恢复出厂的机器的，因为这样就相当于你什么也没恢复。所以请一定不要使用以前备份的配置来恢复刚刷机后，又进行过恢复出厂的路由器。使用【导出设置】备份的配置文件，一般进行了一些设置导致路由器出了问题，将路由器恢复到原厂默认值后，再用备份配置进行恢复，使用备份配置前后，路由器都是同一个版本。

   > **如何恢复出厂**：进入【系统管理 】–【 恢复/导出/上传设置】，点击恢复按钮，记住不要勾选恢复按钮右侧的选择框！！

#### 开始刷机

因为救援模式的存在，加上华硕路由器的固件是双分区结构，所以华硕路由器刷机理论上是刷不死的，即使刷机过程中停电都刷不死！只要开机后有灯亮，那么出现任何无法启动的问题都是能救得活的。所以不论你当前处在什么类型固件、什么固件版本下，都可以尝试一步刷到位：直接刷机到最新的固件！如果能正常通过刷机，成功后进行一次固件双清，达到干净刷机的效果。如果不能通过刷机，救援模式也是分分钟能搞定的事情！所以请不要被下面写得非常详细的刷机流程吓到。

当然，也可以将刷机做到很细致，那么根据你现在的固件，用下面A - E的操作来对号入座把！虽然细致刷机过程也可能发生意外，但是请记住三大法宝：重启、重置、救援模式。

#### A. 原厂固件 → 官改固件：

> 如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好！

1. 在原产固件/原版梅林固件升级页面下直接上传.pkgtb 后缀的官改固件文件；
2. 刷机完成后会自动重启，此时刷机完成；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本。

#### B. 官改固件 → 原厂固件：

> 从官改固件刷回原厂固件，以下第3点或第4点操作，请选择一个来操作。当然你也可以不进行这个操作，让软件中心文件保留在官方固件的JFFS分区，以后你再刷回官改固件，软件中心就会恢复成上次官改的状态。

1. 在官改固件升级页面下直接上传.pkgtb  后缀的华硕原厂固件文件；
2. 刷机完成后固件恢复为官方固件，但是JFFS分区仍然会保留有一些软件中心相关文件；
3. 你可以参考下文重要命令里的**删除软件中心**，将JFFS内残留的软件中心文件删除；
4. 也可以执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框），这样也将清空JFFS内除软件中心外的其它文件

### 注意事项：

1. 刷机后如果界面显示不正常，请使用组合键`ctrl + F5`强制清空浏览器缓存后重试；
2. 强烈建议使用chrome浏览器或者chromium内核的浏览器，以保持最佳兼容性；
3. 单纯的恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框；
