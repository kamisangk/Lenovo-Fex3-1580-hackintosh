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
1. 显卡HD520驱动正常，注入ID 0x19160000  
2. 声卡ALC236驱动正常，注入ID 16  
3. 键盘触摸板正常，均为PS2设备  
4. usb正常，usbinjectall.kext+ssdt_uiac.aml定制  
5. HDMI输出正常  
6. 睡眠唤醒正常  
7. 原生电源管理  
8. 亮度调节  
## 不正常运行列表
1. Intel 网卡WiFi蓝牙全球无解  
2. sd读卡器  
## 四、备注
1. 内存报错需要在smbios添加内存信息才能成功进入clover界面安装。  

