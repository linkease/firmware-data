384_82072（2020年10月12日）
同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.82072。
去除更多哥特（Gothic）风格字体，因为其显示中文的时候字体发虚，实在太丑；
内置软件中心更新至1.6.4，添加实时日志、提升插件安装/卸载速度！详情见： 软件中心更新日志
现在使用RT-AC86U官改固件作为AiMesh节点时，其web后台能正常访问了！
更改软件中心数据库文件夹：jffs/db → jffs/ksdb;
针对RT-AC86U 384_82072第4点更新的说明如下，请仔细阅读：

华硕对AiMesh节点仅开放了固件更新这一个页面功能，这限制得太多了，但是这也是为了避免用户对节点进行设置造成mesh网络出问题；
kooldev将AiMesh节点的web后台访问全部开放了，但是需要提醒大家请尽量不要改动与AiMesh相关的设定，以免影响AiMesh网络的正常工作；
我们开放AiMesh节点的web后台的访问，主要目的是为了大家能在AiMesh节点中使用软件中心，当然你也可以进行一些固件相关的设定，比如无线区域。
需要注意的是因为AiMesh节点本质上是工作在中继模式，而非NAT模式，所以一些透明代理类的插件在AiMesh节点路由上是无法正常工作的，比如xxxx，kp等；
如果你在AiMesh节点中修改了某些系统设置导致AiMesh网络失效，请在开机状态下长按机器后面的reset按钮重置你的AiMesh节点路由，然后用主路由重新添加节点；
AiMesh节点web后台的访问方式：在AiMesh主路由的【网络地图】页面点击【AiMesh节点】图标，然后在页面右侧会出现目前已经连接的AiMesh节点，点击对应节点机器后，会弹出节点信息，信息中会显示该节点机器的ip地址，比如我的是192.168.86.126，然后在浏览器中访问http://192.168.86.126即可访问AiMesh节点路由。