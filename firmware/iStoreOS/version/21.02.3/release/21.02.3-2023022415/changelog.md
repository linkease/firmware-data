# 系统：
更新 r8152 驱动，以支持 RTL8156(B) 方案的 2.5G USB 有线网卡 8156B usb 网卡，奇怪问题，可以获取IP，但不能上网 #211 更新日志 - 20230217 #597 (comment)
修复 Argon 主题 CSS 压缩错误导致的字体异常 后台管理界面字体映射错误 #239 csstidy break font-face openwrt/luci#5067 CSSTIDY: csstidy minifier is outdated and breaks CSS 2.1+ syntax. It is time to phase it out or replace it with a better tool. openwrt/luci#5755
修复 LUCI lua 版本对 ipv6 格式的判断错误 更新日志 - 20230217 #597 (reply in thread)
应用：
# QuickStart：
修复 RAID 扩容时对 RAID 进行分区的严重 BUG（应该对加入陈列的磁盘进行分区）
修复磁盘和分区的空间使用率显示
修复部分插件安装向导状态提示
以下为小伙伴 司波图 反馈 ( https://www.bilibili.com/video/BV1yA411U7Xg ) ：
修复一键配置 Aria2，qBittorrent，Transmission
Aria2 增加一键配置 AriaNg 链接
修复 “内网配置” 修改 IP 以后的状态判断和自动跳转
# 设备：
修复部分设备上一版本固件（20230217）内核配置变化导致的Docker容器启动失败问题