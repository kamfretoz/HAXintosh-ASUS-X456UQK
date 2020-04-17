# HAXintosh for ASUS X456UQK
A collection of Kext and config.plist for my ASUS Laptop

![Alt text](/SCREENSHOTS/rEFInd.png?raw=true "rEFInd Main Screen")

- Laptop Model: ASUS VivoBook X456UQK
- Installer: **Olarila Vanilla Installer**
- macOS Version: Mojave (10.14.6)
- Clover Version: r5112

## System Spec:
* CPU: Intel Core i7-7500U @2.70GHz *(Kabylake)*
* RAM: 12GB DDR4
* iGPU: Intel UHD 620
* dGPU: NVIDIA GeForce 940MX
* Audio: Connexant CX8050
* Wireless: Atheros AR9565
* SSD: ADATA SU650 128GB *(Windows)*
* HDD: HGST HTS541010A9E680 1TB *(Hackintosh and Data)*

## Partition Layout:
```
╭─[~/Documents/EFI]─[kamfretoz@192]─[0]─[64]
╰─[:)] % diskutil list
/dev/disk0 (internal, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *1.0 TB     disk0
   1:                        EFI EFI                     209.7 MB   disk0s1
   2:           Linux Filesystem                         129.2 GB   disk0s2
   3:                  Apple_HFS HAXintosh               118.6 GB   disk0s3
   4:                 Apple_Boot Recovery HD             650.0 MB   disk0s4
   5:       Microsoft Basic Data                         36.5 GB    disk0s5
   6:       Microsoft Basic Data                         17.2 GB    disk0s6
   7:       Microsoft Basic Data DATA                    697.9 GB   disk0s7

/dev/disk1 (internal, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *120.0 GB   disk1
   1:         Microsoft Reserved                         16.8 MB    disk1s1
   2:       Microsoft Basic Data KamFretoZ               120.0 GB   disk1s2
```

## INSTALLED OPERATING SYSTEMS:
* Windows 10 - Vista Edition
* TheHAXintosh (Hackintosh)
* EndeavourOS (Arch Linux)
* Haiku

## **What Works**:
- Quartz Compositor / Core Image
- Audio
- WiFi
- Bluetooth
- Touchpad
- USB 2.0, 3.0 & Type-C
- ASUS ATK (FN Hotkeys)
- Sleep & Shutdown
- Speedstep
- Screen Backlight
- Intel GPU
- SD Card reader
- HDMI & VGA Output
- CPU Power Management

## **What Doesn't**:
- NVIDIA GPU

### Stuff used:
- [RehabMan's AppleBackLightFixer] https://github.com/RehabMan/OS-X-Intel-Backlight
- [AsusSMC] https://github.com/hieplpvip/AsusSMC
- [CPUFriend] https://github.com/acidanthera/CPUFriend
- [VoodooI2C] https://github.com/alexandred/VoodooI2C
- [AppleALC] https://github.com/acidanthera/AppleALC
- [WhateverGreen] https://github.com/acidanthera/WhateverGreen
- [rEFInd-glassy theme] https://github.com/Pr0cella/rEFInd-glassy

- **config.plist** used from Olarila's Clover Patches Collection and Tweaked a bit https://www.olarila.com/topic/5676-folders-for-all-chipsets-clover-and-opencore/
