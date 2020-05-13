# DELL-OptiPlex-7050
适用于DELL-OptiPlex-7050机器的OpenCore引导，适配MacOS10.15.4

* 机器配置	
	* CPU: i7-7700
	* Audio: ALC255
	* Graphics: HD630
  * Monitor: DP 4K monitor

## 调整BIOS 参数
解压EFI-shell.zip到U盘的任意FAT32分区根目录(e.g. 分区:/EFI/BOOT/bootx64.efi),然后重启用UEFI方式启动这个U盘.

开机启动时按F12，选择这个U盘，直接进入GRUB界面

在GRUB界面中输入
setup_var 0x795 0x2  （修改dvmt 为64MB）
setup_var 0x4ED 0x0   （禁用CFG lock）

### 感谢
- Apple
- Dell
