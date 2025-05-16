21.02.2 r16763
发布日期 2022-04-15

系统：

更新QuickStart，支持更丰富的磁盘管理功能
修复某些app安装以后需要重新登录luci才出现菜单的问题
默认禁用 net.bridge.bridge-nf-call-iptables，只对Docker的网络接口启用，防止NAT反射（回流）失效
默认桥接lan
修复argon主题下载bing壁纸可能卡住的问题
Docker修改数据目录时重启
添加OpenAppFilter，提高管控>网址过滤的性能