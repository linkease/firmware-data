# 系统：
固件集成 kmod-inet-diag 内核模块 添加kmod-inet-diag，openclash的process-name规则依赖此前置 #611 我的是树莓派4b, 安装passwall时提示各缺少依赖iptables-mod-socket, 安装openclash提示缺少kmod-inet-diag，hello world创建节点时无法通过剪切板导入节点。目前只有SSR好用。 #581
提高内核兼容性，以便安装 OpenWRT 预编译的内核模块，可自行在软件包中安装 iscsi，mpls，openvswitch 等驱动 （x86, rk33xx, rpi4等使用5.4内核的设备）
# 应用：
QuickStart：

修复旁路由模式切换以后默认网关没有立即生效的问题
修复Docker的开关 Docker停止失败 #633
修复静态IP联网时，自动获取DNS选项依然可用的问题
网络向导：切换非旁路由联网模式时，如果之前旁路由模式关闭了DHCP服务，就显示一个重新打开DHCP服务的开关
网络向导：旁路由向导在配置完成时提醒用户后续操作，以及跳转按钮使用旁路由IP
iStore：

增加了 kmod-ipt-socket，iptables-mod-socket 兼容模块 我的是树莓派4b, 安装passwall时提示各缺少依赖iptables-mod-socket, 安装openclash提示缺少kmod-inet-diag，hello world创建节点时无法通过剪切板导入节点。目前只有SSR好用。 #581 R2C测试固件内核iptables-mod-socket不可用 #570
# 设备：
RK3568系列： 提高千兆网口的性能（包括R5S，R68s等），测试自建 PPPOE 服务可以跑满千兆 r5s 最新固件 跑不满千兆 #518
R4S/R66s：修复从某些高速SD卡启动以后，软重启失败问题（软件降级到低速卡） Rockchip方案机型从高速sd卡启动后软重启失败 #565