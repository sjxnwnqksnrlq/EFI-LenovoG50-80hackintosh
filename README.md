# EFI-LenovoG50-80hackintosh
联想G50-80 黑苹果 EFI 文件。适配 macOS 版本为 10.13.6--10.14 Developer Beta 6（最新版）

使用之前，请务必重新 generate 序列号，方法为 Clover Configurator 中选择 SMBIOS-找到那个箭头的地方，选择 MacBook Pro 12,1 就可以了。

已经完美的功能包括：声卡，显卡，网卡，变频，睡眠，无线网卡（更换 BCM94352z，记住联想笔记本需要刷白名单破解）

暂不完美的包括：iMessage，FaceTime，Handoff 部分高级功能（和网卡有关，无解）

2018.08.07 修改：加入 USB 3.0 patch

2018.08.09 修改：微调 ApplePS2smarttouchpad 手势，让它更接近白苹果，info.plist 为略微自定义的触控板配置文件（虽然仍然建议购买 Magic Trackpad 2）

https://osxlatitude.com/forums/topic/5966-details-about-the-smart-touchpad-driver-features/
注意：右键需要设定为 33.

2018.08.11 修改：如果要使用 VGA 输出，请使用 16160002 的 ig 作为你的显卡 ig。

2018.08.18 修改：更新了一揽子驱动，使用 Whatevergreen 代替 IntelGraphicsFixup。更换了 BCM94360CS2 MacBook Air 拆机网卡，去掉了蓝牙和 Wi-Fi的相关 patch。
