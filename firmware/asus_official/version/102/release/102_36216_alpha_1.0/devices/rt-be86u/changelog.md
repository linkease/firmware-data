**更新日志：**

1. 基于RT-BE86U官方最新源代码制作：GPL_RTBE86U_300610236216；
2. 添加koolcenter软件中心支持，支持45款左右的插件；
3. 彻底禁用华硕自带的固件检测更新；
4. 禁用了国内用户用不到的Alexa和IFTTT功能；
5. 移除了官方固件里特别丑且显示效果发虚的Gothic字体；
6. 添加了更多的busybox组件，以适应软件中心及插件需要
7. 添加了ipset，base64，tproxy，wan-start，nat-start等功能
8. 官改固件登陆后默认进入【网络地图】，且右侧边栏显示CPU内存等状态；
9. RT-BE86U作为5.04behnd.4916平台，兼容hnd/axhnd平台的所有插件；

##### 已知问题

1. 当开启vlan后，dnsmasq的postconf功能有问题，这可能会影响一些需要自定义dnsmasq配置的插件

	在这个问题解决之前，建议使用这些插件的用户暂时不使用vlan划分功能