21.02.3 r16818
发布日期 2022-12-02

系统：

LUCI 合并上游的修改，区分 http 和 https 的 cookie，避免 cookie 策略导致 http 无法登录
增加 curl 的容错机制，防止用户部分升级 curl 相关包导致 curl 不可用
应用：

易有云：修复配置文件错误导致绑定信息丢失