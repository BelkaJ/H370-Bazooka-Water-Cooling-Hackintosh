# H370 Bazooka Water Cooling Hackintosh
![It Works For Me](https://img.shields.io/badge/It%20Works-For%20Me™-green)
[![MacOS Ventura](https://img.shields.io/badge/macOS-13.6-9cf)](https://www.apple.com/macos/ventura/)
[![OpenCore](https://img.shields.io/badge/OpenCore-0.8.6-f95)](https://github.com/acidanthera/OpenCorePkg/releases/0.8.6)

I built an open-frame water-cooling wall desktop on a Thermaltake Core P3 case, mainly for decorative and aesthetic purposes.

<img src="Images/Light2.jpg"  width="500"/>


I use my computer for everyday work.  I am not a game player and  I do not need much computing power. Therefore, I used some parts of the old Hackintosh/Windows desktop (dualbooting) to upgrade the system to Ventura and the bootloader to OpenCore.

Windows were installed on the first partition of the disk, and MacOS was installed on the second partition according to Dortania's guide.

I used EFI and settings were based on ideas of DERBALKON project for MSI B360M https://github.com/derbalkon/B360M-CoffeeLake-Hackintosh (THANK YOU!)

MacOS was installed without any problems. I introduced a boot menu in the config.plist to enable DualBooting. OpenCore starts from USB.

<img src="Images/Dual boot.png" />


|                |                                                   |
| ------------: | :------------------------------------------------- |
|         Board | MSI® H370M Bazooka                                 |
|           CPU | Intel® Core™ i5-8500                               |
|        Memory | Corsair 4 x 8GB (DDR4 2666MHz)                     |
|           SSD | Adata SSD  M.2 256GB                               |
|  Graphic Card | Asus Radeon™ RX460 2GB x8                          |
| Wireless Card | Broadcom® BCM94360 AliExpress (with Bluetooth 4.0) |
|       Monitor | Dell 1600x1200 LCD Monitor                         |
                           

I adapted the system to my hardware:

- kext Ethernet 1GB Realtec RTL8111

- audio codec 87

- PCI entries for the Raedon RX 460 audio decoder, Wifi/BT Broadcom BCM3640, Realtec RTL8111

- I mapped the USB following the guide at: https://github.com/corpnewt/USBMap. I did not manage to map the  USB3 port MB to the front panel, as my MB has a damaged slot.

- SMBIOS iMac 19.2

What is not working:

PowerOff via on/off button front panel - I don't know how to fix it
The waking up  only works via the on/off front panel - but for me this is not a disadvantage because the fans do not turn on when the keyboard and mouse are hit.


What is working:
Everything apart from above, INCLUDING APPLE MUSIC AND APPLE TV!!!! 
There are no DRM problems

