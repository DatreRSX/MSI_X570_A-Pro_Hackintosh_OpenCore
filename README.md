# Hackintosh Guide for **MSI X570 A-Pro Motherboard**

**This guide it's updated to OpenCore 0.9.8 and tested on Sonoma**
Now Works with Seqoia ,must update kext and kernel patches
## Specs:
| Component | Brand |
|:--- |:---:|
| Motherboard:  | Msi A-Pro X570 |
| CPU: | AMD Ryzen 5 5600X |
| GPU: | Msi Mech 6700XT 12GB |
| Memory: | Vengeance 16gb 3200MHz 16GB x4|
| Audio: | Realtek ALC1220 |
| Ethernet: | Realtek 8111H |
| Power Supply: | NOX URANO 650W |
| Case: | Tailus Chronos |

These are all the external ports of the Motherboard. (**They all work**):

![MSI X570 A-PRO Layout](/Docs/Images/Guide/IO_layout.png)

### Working
- [x] **Tested with macOS Big Sur to Ventura Beta 8**
- [x] **Bluetooth:** ([With a USB adapter](amazon.com))
- [x] **USB:** All internal and external ports (Thanks to SSDT-EC-USBX.aml)
- [x] **Ethernet:** Realtek RTL8111 (Thanks to RealtekRTL8111.kext)
- [x] **HDMI, DisplayPort:** Works perfect. 
- [x] **Shutdown/Restart/Sleep/Wake:** Yes

### Not working
- Continuity Features
- Some software due the limitations of an AMD CPU.

## Important
---
Due to a NootRX bug, your installation will not boot on installation and first boot, you will have to perform installation and first boot without graphics acceleration (enable whatgreen kext in config.plist)

Whatevergreen kext will not be in this repository so you will have to download it, in addition to adding it to your config.plist

[](https://github.com/acidanthera/WhateverGreen)

**DO NOT USE Whatevergreen and NootRX at the same time, these two kexts are incompatible if run at the same time**

Once the installation is finished, delete Whateveergreen kext from the kexts folder and its config.plist, you won't need it anymore.
Once you have entered the desktop for the first time you can enable NootRX kext in config.plist
---

# INSTALLATION GUIDE

---

## Making the Booteable USB

### From macOS:
[**Link to Apple's Guide**](https://support.apple.com/en-us/HT201372)

### From Windows:

[**Link to Dortania's Guide**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html)

### From Linux:

[**Link to Dortania's Guide**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/linux-install.html)


---

# BIOS Settings:
- Make Sure you have [Latest BIOS](https://www.msi.com/Motherboard/support/X570-A-PRO#down-bios)
- After Updating the BIOS, you need some configuration to working.

---

# Credits

[Apple](https://apple.com) (macOS)

[OpenCore Team](https://github.com/acidanthera/OpenCorePkg) (Bootloader)

[Dortania](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/amd.html#starting-point) (Guide)

---
# Thanks
**RobyRew for doing  the EFI folder , configurations in APCI and Config.plist**

[](https://github.com/RobyRew/MSI_X570_A-Pro_Hackintosh_OpenCore)https://github.com/RobyRew/MSI_X570_A-Pro_Hackintosh_OpenCore

NootRX to give support on NAVI 21 22 23 arquitectures 

https://github.com/ChefKissInc/NootRX

---

