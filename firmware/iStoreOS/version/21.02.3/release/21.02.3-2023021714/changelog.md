# 系统：
提高内核兼容性，以便安装 OpenWRT 预编译的内核模块 （x86, rk33xx, rpi4等使用官方内核的设备） 希望增加对UVC 相机设备的支持 #579
修复 luci 的 lua 版本的条件判断异常，增加错误字段高亮显示 udpxy插件网页版无法配置续订参数 linkease/doc.linkease.com#81 luci-app-udpxy: Multicast subscription renew cannot save openwrt/luci#5705
修复沙箱提交以后，overlayfs 可能出现冗余的 whiteout 标记的问题
# 设备：
x86：
集成新 mt76 wifi 驱动，以支持 mt7921 的 AP 模式 （5G 频段有些信道无法启动 AP ，建议使用默认值）
集成 Intel AX201 wifi 驱动（不支持 AP 模式）
R2S/R2C：
根据 PHY 芯片 ID 自动调整 MAC 的 delay 值，可能有助于提高网络稳定性 更新日志 - 20230203 #573 (comment)