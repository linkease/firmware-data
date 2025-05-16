21.02.2 r16767
发布日期 2022-04-22

系统：

防止网络重启导致docker的网络桥docker0被删除
限制luci实时信息网络连接条目数最多1000条，防止rpcd服务被下线
upnp支持无公网ip的转发，暂时需要命令开启uci set upnpd.config.force_forwarding=1 ; uci commit upnpd
其他：清理argon登录界面不需要的代码，更新quickstart