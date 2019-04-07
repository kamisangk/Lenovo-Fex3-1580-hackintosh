# 一、机型配置
| 硬件  | 型号  |
| ------------ | ------------ |
| 处理器名称  |	DualCore Intel Core i7-6500U, 2666 MHz (27 x 99)   |
|  	主板名称  |	Lenovo Flex 3-1580   |
| 系统内存  |  	7989 MB (DDR4 SDRAM) |
|  显示适配器 |   Intel(R) HD Graphics 520 (1 GB)|
| 	显示器    |  	LG Philips LP156WF6-SPK1 [15.6" LCD] |
| 音频适配器   | 	Realtek ALC236  |
|  硬盘 | 	ACSC4M512S25 STAT3 (476 GB)  |
|  网络适配器 |   Realtek PCIe GBE Family Controller|
|  WiFi | 	Intel(R) Dual Band Wireless-AC 3168  |
# 二、安装之前BIOS设置
	-Disabled discrete GPU  
	-Disabled Intel Virtualization  
	-Disabled Intel Platform Trust Technology  
	-Disabled Secure Boot  
	-Boot MODE → Legacy Support  
# 三、运行状态
## 正常运行列表
	显卡HD520驱动正常，注入ID 0x19160000  
	声卡ALC236驱动正常，注入ID 16  
	键盘触摸板正常，均为PS2设备  
	usb正常，usbinjectall.kext+ssdt_uiac.aml定制  
	HDMI输出正常  
	睡眠唤醒正常  
	原生电源管理  
	亮度调节  
## 不正常运行列表
	Intel 网卡WiFi蓝牙全球无解  
	sd读卡器  
# 四、DSDT补丁
## 对DSDT打下列补丁  
	Fix system_HPET  
	Fix system_IMEI  
	Fix system_IRQ  
	sys system_OSYS_win10  
	Fix system_WAK Arg0 V2  
	Fix system_RTC 
	Fix system_SMBUS  
	Fix system_PNOT/PPNT  
	Fix usb_prw_0x6d_xhc  
	Fix Mutex with non-zero synclevel  

## 四、备注
	 内存报错需要在smbios添加内存信息才能成功进入clover界面安装。  
	 



