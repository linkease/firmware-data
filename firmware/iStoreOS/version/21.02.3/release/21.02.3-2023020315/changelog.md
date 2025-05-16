# 系统：
修复启动时 PARTUUID 冲突可能导致 overlay 挂载失败的问题
修复 PARTUUID 冲突可能导致 boot 分区挂载失败或者固件升级时写错 boot 分区的问题 error:root not found #535
修复 lua 升级可能导致 argon 主题异常崩溃的问题
# 设备：
x86：修复某些设备在 GRUB 界面不自动启动 iStoreOS 的问题（倒计时失效） x86_1216版本引导时卡在GNU GRUB界面，无法自动引导iStoreOS #558
R2S：固件支持 R2C 的网卡 希望能增加对友善 NanoPi R2C 的支持 #309 希望r2s istore固件加入yt8521s驱动，现在我的r2cplus只能单臂路由，谢谢 #358 什么时候出R2C的固件呀，现在我R2C只能当单臂路由来用 #439
# 应用：
QuickStart：修复多个 RAID 功能相关bug istorex 对 raid 支持不友好 linkease/nas-packages-luci#54
QuickStart：修复 docker 根目录状态的判断
QuickStart：修复 x86 安装器安装以后 GPT 分区表可能无效的问题 X86 版 1216，在U盘安装完毕后，重启后拔掉U盘，卡在启动界面 #556 安装后拔去U盘重启报错i915 0000:00:02.0: Failed to load DMC firmware i915/kbl_dmc_ver1_04.bin. Disabling runtime power management. #557
QuickStart：修复 efi 固件分区格式化系统盘剩余空间可能失败的问题 无法格式化+挂载硬盘 #408
QuickStart：x86 安装器跳过小于 2.5GiB 的硬盘
QuickStart：提高 lean's LEDE 固件的兼容性 最新的大雕源码编译 首页不显示磁盘信息，之前配置了docker配置文件可以显示，这次不显示了 linkease/nas-packages-luci#55