# 已知问题：

R5S/R5C的led灯无效，下个版本会解决
ddns插件未集成腾讯（dnspod），临时解决方法：从软件包中安装 ddns-scripts-dnspod
Transmission无法启动，临时解决方法：从软件包中安装 libmbedtls
aria2无法启动，卸载重装即可
如果之前版本使用nginx作为luci的服务可能导致后台无法打开，卸载重装nginx相关的包即可（ssh或者ttyd终端（浏览器打开7681端口），登录以后执行opkg remove --force-removal-of-dependent-packages --autoremove nginx-util; opkg update ; opkg install luci-nginx）。
如果遇到问题，先别急着反馈，试试恢复出厂设置或者重新刷机能不能重现。很多问题只是因为之前版本的时候，自己手动升级了系统的软件包，在新版本中不兼容。不管任何时候，都尽量别去升级系统软件包，以免升级到官方有bug或者不兼容的版本，而且还影响以后的固件升级，如果手痒的话，在沙箱模式里面玩。 https://doc.linkease.com/zh/guide/istoreos/question.html