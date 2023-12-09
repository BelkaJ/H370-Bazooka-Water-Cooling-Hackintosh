# H370 Bazooka Water Cooling Hackintosh

I built an open-frame water-cooling wall desktop on a Thermaltake Core P3 case, mainly for decorative and aesthetic purposes.

I use my computer for everyday work.  I am not a game player and  I do not need much computing power. Therefore, I used some parts of the old Hackintosh/Windows desktop (dualbooting) to upgrade the system to Ventura and the bootloader to OpenCore.

Windows were installed on the first partition of the disk, and MacOS was installed on the second partition according to Dortania's guide.

I used EFI and settings were based on ideas of DERBALKON project for MSI B360M https://github.com/derbalkon/B360M-CoffeeLake-Hackintosh (THANK YOU!)

MacOS was installed without any problems.


I adapted the system to my hardware:

- kext Ethernet 1GB Realtec RTL8111

- audio codec 87

- PCI entries for the Raedon RX 460 audio decoder, Wifi/BT Broadcom BCM3640, Realtec RTL8111

- I mapped the USB following the guide at: https://github.com/corpnewt/USBMap. I did not manage to map the  USB3 port MB to the front panel, as my MB has a damaged slot.

- I introduced a boot menu in the config.plist to enable DualBooting. OpenCore starts from USB.

- SMBIOS iMac 19.2

What is not working:

PowerOff via on/off button front panel - I don't know how to fix it
The waking up  only works via the on/off front panel - but for me this is not a disadvantage because the fans do not turn on when the keyboard and mouse are hit.


What is working:
Everything apart from above, INCLUDING APPLE MUSIC AND APPLE TV!!!! 
There are no DRM problems

