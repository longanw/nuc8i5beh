# NUC8i5beh黑苹果EFI文件
`Yale Wei 更新于2023-06-13`

![Catalina](./pic/AboutThisMac_10.15.7.png)

[English](./README.md) | 简体中文  
[![Github](https://img.shields.io/badge/Github-blue.svg)](https://github.com/longanw/nuc8i5beh) [![Gitee](https://img.shields.io/badge/Gitee-brightgreen.svg)](https://gitee.com/yalewei/nuc8i5beh)

#### 简介
豆子峡谷NUC8i5beh的黑苹果EFI配置文件集，同时支持Catalina和Monterey启动，目前主力系统为Catalina 10.15.7。其中的intel WIFI (AirportItlwm.kext)、蓝牙 (IntelBluetoothFirmware.kext)和声卡 (AppleALC.kext)均采用精简编译版（仅保留NUC8i5beh设备驱动，勿用于其他黑果设备）以减少体积，其他资源均来自因特网。

附后**常用工具**是仿照维奇编写的在线安装工具，可用于macOS和windows系统环境下的恢复和在线安装U盘制作，无需下载完整镜像，搭配适合机器的EFI配置文件集，可方便安装对应机型的各个版本的苹果系统，欢迎体验及反馈。

#### 状态：进行中
[![ThinkPad](https://img.shields.io/badge/NUC-NUC8i5BEH-blue.svg)](https://ark.intel.com/content/www/cn/zh/ark/products/126148/intel-nuc-kit-nuc8i5beh.html?wapkw=nuc8i5beh) [![release](https://img.shields.io/badge/Download-latest-brightgreen.svg)](https://github.com/longanw/nuc8i5beh/releases) [![OpenCore](https://img.shields.io/badge/OpenCore-0.9.3-blue.svg)](https://github.com/acidanthera/OpenCorePkg/releases/latest) [![itlwm](https://img.shields.io/badge/itlwm-2.2 stable-blue.svg)](https://github.com/OpenIntelWireless/itlwm/releases) [![MacOS Catalina](https://img.shields.io/badge/macOS-10.15.7-brightgreen.svg)](https://www.apple.com/macos/catalina/) [![MacOS Monterey](https://img.shields.io/badge/macOS-12.6-blue.svg)](https://www.apple.com/macos/monterey/) [![MacOS Ventura](https://img.shields.io/badge/macOS-13.4-brightgreen.svg)](https://www.apple.com/macos/ventura/)

#### NUC配置表

| 组件名称          | 型号规格                                 |
| ---------------- | ---------------------------------------|
| CPU              | Intel® Core™ i5-8259U                  |
| iGPU             | Intel Iris® Plus 655                   |
| Lan              | Intel I219-V                           |
| Audio            | Realtek ALC235                         |
| Ram              | Kingston 16Gb ddr4 2400 Mhz            |
| Wifi + Bluetooth | Intel® Wireless-AC 9560 + Bluetooth 5.0|
| Nvme             | INTEL 760P 512GB                       |
| SSD              | NONE                                   |
| Card Reader      | microSDXC Card Reader                  |
| SMBios           | MacMini8,1                             |
| BootLoader       | OpenCore 0.9.3                         |
| BIOS             | 090                                    |

#### 驱动情况

- [x] Intel Iris® Plus 655 iGPU HDMI/DP Output
- [x] ALC235 Internal Speakers
- [x] ALC235 HDMI/DP Audio Output
- [x] All USB Ports 
- [x] SpeedStep / Sleep / Wake
- [x] Intel® Ethernet Connection I219-V
- [x] Thunderbolt 3 port
- [x] Intel® Wireless-AC 9560 + Bluetooth 5.0
- [x] microSDXC Card Reader
- [x] NVRAM

#### BIOS设置
```
Devices -> USB -> Port Device Charging Mode: off
Devices -> USB -> USB Legacy -> Disabled
Devices -> Video -> IGD Minlmum Memory  ->64MB
Devices -> Video -> Aperture Size  ->256MB
Devices -> Video -> Primary Video Port  -> HDMI
Devices -> Video -> Secondary Video Port -> None
Security -> Thunderbolt Security Level: Legacy Mode
Power -> Wake on LAN from S4/S5: Stay Off
Boot -> Boot Configuration -> Network Boot: Disable
Boot -> Secure Boot -> Disable
```
#### 存在问题
- HDMI接口输出可能存在闪屏现象，需换根品质好的连接线应该可以解决；
- 采用type-C转DP线输出，偶尔会在开机或者使用过程中出现无输出情况，目前采用重启显示器电源解决，具体原因不明。

#### 常用工具

| 名称 | Git 链接 | 主要功能 |
| ---| --- | --- |
| GenSMBIOS| [link](https://github.com/corpnewt/GenSMBIOS) | 生成三码，白嫖党专用 |
| ssdtPRGen| [link](https://github.com/Piker-Alpha/ssdtPRGen.sh) | CPU变频生成脚本 |
| ProperTree| [link](https://github.com/corpnewt/ProperTree) | plist编辑利器 |
| MacInstaller| [link](https://github.com/longanw/nuc8i5beh/blob/master/tools/MacInstaller.zip) | 系统恢复兼做在线系统安装U盘用脚本   |
| BT-LinkeySync| [link](https://github.com/digitalbirdo/BT-LinkkeySync) | 生成双系统蓝牙鼠标共用配置脚本 |

#### 赞助，一分也是爱！

| 微信支付 | 支付宝 | 
| ---| --- |
| ![WePay](./pic/WePay.png) | ![alipay](./pic/Alipay.png) |

#### 感谢名单

- [Apple](https://www.apple.com) 的macOS
- [Intel](https://ark.intel.com/content/www/cn/zh/ark/products/series/129705/intel-nuc-kit-with-8th-generation-intel-core-processors.html) 第八代智能英特尔® 酷睿™ 处理器的NUC 套件
- [Acidanthera](https://github.com/acidanthera) 维护的项目
- [Rehabman](https://github.com/RehabMan) 和 [黑果小兵](https://github.com/daliansky) 维护的项目
- [zxystd](https://github.com/OpenIntelWireless/itlwm) 开发的Intel WIFI和Bluetooth驱动
- [zearp](https://github.com/zearp/Nucintosh) 精简编译的Intel WIFI和Bluetooth驱动
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/) 的OpenCore安装指引
- [码云](https://gitee.com) 
- [github.com](https://github.com) 



