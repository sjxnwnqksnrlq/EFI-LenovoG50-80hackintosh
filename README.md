# EFI-LenovoG50-80hackintosh
联想G50-80 黑苹果 EFI 文件。适配 macOS 版本为 10.13.6--10.14 Developer Beta 6（最新版）
    已经完美的功能包括：
      声卡，显卡，网卡，变频，睡眠，无线网卡（更换 BCM94352z，记住联想笔记本需要刷白名单破解）
    暂不完美的包括：
      iMessage，FaceTime，Handoff 部分高级功能（和网卡有关，无解）
2018.08.07 修改：
    加入 USB 3.0 patch，感谢某 QQ 群群友指导：：
    		<key>KextsToPatch</key>
		<array>
			<dict>
				<key>Comment</key>
				<string>change 15 port limit to 24 in XHCI kext</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				g710////EA==
				</data>
				<key>InfoPlistPatch</key>
				<false/>
				<key>MatchOS</key>
				<string>10.12.x</string>
				<key>Name</key>
				<string>AppleUSBXHCIPCI</string>
				<key>Replace</key>
				<data>
				g710////Gw==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>change 15 port limit </string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				g32MEA==
				</data>
				<key>InfoPlistPatch</key>
				<false/>
				<key>MatchOS</key>
				<string>10.13.0-10.13.3</string>
				<key>Name</key>
				<string>AppleUSBXHCIPCI</string>
				<key>Replace</key>
				<data>
				g32MGw==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>Change 15 port limit to 26 in XHCI kext</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				g32UDw==
				</data>
				<key>InfoPlistPatch</key>
				<false/>
				<key>MatchOS</key>
				<string>10.13.4-10.13.5</string>
				<key>Name</key>
				<string>AppleUSBXHCI</string>
				<key>Replace</key>
				<data>
				g32UGw==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>change 15 port limit to 26 in XHCI kext</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				g32IDw==
				</data>
				<key>InfoPlistPatch</key>
				<false/>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Name</key>
				<string>AppleUSBXHCI</string>
				<key>Replace</key>
				<data>
				g32IGw==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>change 15 port limit to 26 in XHCI kext</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				g/sPD4MDBQAA
				</data>
				<key>InfoPlistPatch</key>
				<false/>
				<key>MatchOS</key>
				<string>10.14</string>
				<key>Name</key>
				<string>AppleUSBXHCI</string>
				<key>Replace</key>
				<data>
				g/sPkJCQkJCQ
				</data>
			</dict>
		</array>
