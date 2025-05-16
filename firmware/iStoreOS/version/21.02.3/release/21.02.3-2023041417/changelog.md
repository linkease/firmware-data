# 设备：
rk3568机型：内核开启 ipv4 的策略路由 uu加速器手机app提示组件初始化失败 #584 R68S在使用tproxy模式时出错，提示 RTNETLINK answers: Address family not supported by protocol。 #703
r4s/r2s/rpi4：从固件移除部分用不上的内核模块（可能只有x86平台才能用），如有需要可从软件包安装或者提issue
r2s：修复 LAN 口相关的多个问题：部分机器不识别，频繁掉线，跑不满千兆。 r2s 跑不满千兆 #690 R2S的lan口经常掉线 #696
x86 和 rk3568 机型 有 22.03.4 的测试固件，详情看 #716 。
x86 测试固件支持了 N5105 的硬解，从iStore安装jellyfin插件，并且部署以后，在jellyfin的“控制台”-“播放”选择 QuickSync 转码器，剩下的硬解选项除了 AV1 以外都可以勾选上。