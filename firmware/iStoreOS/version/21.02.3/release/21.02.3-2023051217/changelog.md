# 应用：
QuickStart：
修复某些情况下首页显示的本地时间错误的问题 首页系统时间比本地时间快8小时 #737
# 设备：
x86：支持了Ventoy多镜像U盘启动，7z/gzip解压后放在U盘里即可使用，无需额外处理镜像文件 使用ventoy打开istoreos的ISO和img都会卡在new full-speed USB device number 4 using ci_hdrc #431
rk3568:
打开openssl优化选项，提高加解密性能
优化网卡CPU调度，提高性能和稳定性
增加22.03.4测试固件，支持部分无线网卡 （非此固件，需手动更新，详情）