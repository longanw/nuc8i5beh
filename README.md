# NUC8i5beh黑苹果EFI文件

#### 介绍
豆子峡谷NUC8i5beh的黑苹果efi文件，MacOS版本为Catalina 10.15.7，相关资源来自因特网。

#### 状态：进行中
[![ThinkPad](https://img.shields.io/badge/NUC-NUC8i5BEH-blue.svg)](https://ark.intel.com/content/www/cn/zh/ark/products/126148/intel-nuc-kit-nuc8i5beh.html?wapkw=nuc8i5beh) [![release](https://img.shields.io/badge/Download-latest-brightgreen.svg)](https://gitee.com/yalewei/nuc8i5beh/releases) [![OpenCore](https://img.shields.io/badge/OpenCore-0.7.1-blue.svg)](https://github.com/acidanthera/OpenCorePkg/releases/latest) [![itlwm](https://img.shields.io/badge/itlwm-2.0-blue.svg)](https://github.com/OpenIntelWireless/itlwm/releases) [![MacOS Catalina](https://img.shields.io/badge/macOS-10.15.7-brightgreen.svg)](https://www.apple.com/macos/catalina/) [![MacOS Big Sur](https://img.shields.io/badge/macOS-11.4-purple.svg)](https://www.apple.com/macos/big-sur/)

#### NUC配置表

| 组件名称          | 型号规格                                  |
| ---------------- | ---------------------------------------|
| CPU              | Intel® Core™ i5-8259U                  |
| iGPU             | Intel® Iris® Plus 655                  |
| Lan              | Intel I219-V                           |
| Audio            | Realtek ALC235                         |
| Ram              | Kingston 16Gb ddr4 2400 Mhz           |
| Wifi + Bluetooth | Intel® Wireless-AC 9560 + Bluetooth 5.0|
| Nvme             | INTEL 760P 512GB                       |
| SSD              | NONE                                   |
| Card Reader      | microSDXC Card Reader                  |
| SMBios           | MacMini8,1                             |
| BootLoader       | OpenCore 0.7.1                         |


#### 驱动情况

- [x] Intel Intel® Iris® Plus 655 iGPU HDMI/DP Output
- [x] ALC235 Internal Speakers
- [x] ALC235 HDMI/DP Audio Output
- [x] All USB Ports 
- [x] SpeedStep / Sleep / Wake
- [x] Intel® Ethernet Connection I219-V
- [x] Thunderbolt 3 port
- [x] Intel® Wireless-AC 9560 + Bluetooth 5.0
- [x] NVRAM

#### 存在问题
- HDMI接口输出存在闪屏现象，换了几根在Windows下可用的HDMI线（可以4K@60Hz）均未解决，用type-C转DP接口一切正常，不知道是否与显示器Dell U2718Q兼容有关；
- 读卡器换了很多驱动均不可用。

#### 感谢名单

- [Apple](https://www.apple.com) 的macOS
- [Intel](https://ark.intel.com/content/www/cn/zh/ark/products/series/129705/intel-nuc-kit-with-8th-generation-intel-core-processors.html) 第八代智能英特尔® 酷睿™ 处理器的NUC 套件
- [Acidanthera](https://github.com/acidanthera) 维护的项目
- [Rehabman](https://github.com/RehabMan) 和 [黑果小兵](https://github.com/daliansky) 维护的项目
- [@zxystd](https://github.com/OpenIntelWireless/itlwm) 开发的Intel WIFI和Bluetooth驱动
- [@zearp](https://github.com/zearp/Nucintosh) 精简编译的Intel WIFI和Bluetooth驱动
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/)的OpenCore安装指引
- [码云](https://gitee.com) 
- [github.com](https://github.com) 



