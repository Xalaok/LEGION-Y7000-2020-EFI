# LEGION-Y7000-2020-EFI
 Y7000 2020 黑苹果 EFI

Y7000 系列通用安装教程：<https://www.xalaok.top/post/hackintosh/>

OpenCore 版本：0.8.8

我的电脑信息：
- CPU：Intel Core i7-10750H 2.60GHz
- GPU：Nvidia GeForce GTX1650Ti
- RAM：Kingston 16 GB DDR4 3200MHz
- 固态硬盘：Lenovo SL700 SATA3 240GB
- 无线网卡：Intel Wi-Fi 6 AX201 160MHz

如果和我的配置一样（硬盘除外），且安装的 macOS 版本也是 Ventura，那么可以直接使用本 EFI，如果不是 Ventura 需要更换无线网卡驱动（方法参见[教程](https://www.xalaok.top/post/hackintosh/)），如果配置不同需要自行根据[教程](https://www.xalaok.top/post/hackintosh/)配置 EFI

**重要:** 如果是自带 PM981、PM981a、镁光、海力士固态需要自行插别的硬盘，且需屏蔽自带固态，具体方法也在[教程](https://www.xalaok.top/post/hackintosh/)

## 说明

### 正常工作的功能

- UEFI 通过 Clover/OpenCore 启动
- 支持任意版本系统 OTA 升级到最新系统
- 内置键盘以及数字键盘
- 原生 USB3.0/USB2.0
- AppleHDA 原生音频，包括耳机
- 内置摄像头
- 原生电源管理
- 电池状态
- 背光控制
- 背光键盘
- 核显驱动（独显已屏蔽）
- 有线以太网卡
- App Store
- CPU 变频
- 熄屏唤醒
- 无线网络
- 蓝牙
- 触控板 （全系支持全手势）
- 随航（有线/无线）
- 4K 屏幕（[教程](https://github.com/xiaoMGitHub/LEGION_Y7000Series_Hackintosh/tree/master/4K_Display_Config)）
- iMessage/FaceTime
- 休眠唤醒（hibernatemode 25）

### 不能正常使用的功能

- 睡眠唤醒（原作者说鼠标，键盘、电源键唤醒均正常，但实测我的型号不正常😭）
- HDMI，因为 HDMI 端口连接到已禁用的 Nvidia 卡