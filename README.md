# EFI-LenovoG50-80hackintosh
驱动链接：

https://github.com/acidanthera/WhateverGreen/releases

https://github.com/acidanthera/AppleALC/releases

https://github.com/acidanthera/Lilu/releases

https://bitbucket.org/RehabMan/os-x-fake-pci-id/downloads/

https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/

https://bitbucket.org/RehabMan/os-x-acpi-battery-driver/downloads/

https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/

https://bitbucket.org/RehabMan/os-x-realtek-network/downloads/

联想 G50-80 黑苹果 EFI 文件。核心配置为 Intel Core i5 5200U with HD5500，RTL8111 有线网卡，Conexant 20751/2 声卡，独立显卡已屏蔽，无线网卡先更换为 BCM94352z，目前已经更换为 MacBook Air 拆机网卡 BCM94360CS2.

适配 macOS 版本为 10.13.6（17G65)--10.14 Developer Beta (18A371a)

使用之前，请务必重新 generate 序列号，方法为 Clover Configurator 中选择 SMBIOS-找到那个箭头的地方，选择 MacBook Pro 12,1 就可以了。

已经完美的功能包括：声卡，显卡，网卡，变频，睡眠，无线网卡

暂不完美的包括：iMessage，FaceTime，Apple Watch 解锁 Mac（系统信息显示支持，但是偏好设置没有相关选项）

2018.08.07 修改：加入 USB 3.0 patch

2018.08.09 修改：微调 ApplePS2smarttouchpad 手势，让它更接近白苹果，info.plist 为略微自定义的触控板配置文件（虽然仍然建议购买 Magic Trackpad 2）

https://osxlatitude.com/forums/topic/5966-details-about-the-smart-touchpad-driver-features/
注意：右键需要设定为 33.

2018.08.11 修改：如果要使用 VGA 输出，请使用 16160002 的 ig 作为你的显卡 ig。

2018.08.18 修改：更新了一揽子驱动，使用 Whatevergreen 代替 IntelGraphicsFixup。更换了 BCM94360CS2 MacBook Air 拆机网卡，去掉了针对 BCM94352z 网卡的蓝牙和 Wi-Fi 的相关 patch。

https://blog.daliansky.net/Broadcom-BCM94352z-DW1560-drive-new-posture.html

![图片](https://github.com/sjxnwnqksnrlq/EFI-LenovoG50-80hackintosh/blob/master/images/image.png)

2018.08.21 修改：使用了一种全新的方法，来解决升级到最新 Mojave Beta 版 DVMT 补丁失效的问题。处于容错考虑，之前的 DVMT kextstopatch 仍然保留，只是 disable 掉。

https://www.insanelymac.com/forum/topic/334899-intel-framebuffer-patching-using-whatevergreen/
