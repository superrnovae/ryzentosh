**macOS versions**: 10.15.1 - 11.1

**OpenCore version**: [0.6.5](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.6.5)

**BIOS version**: [7C02v3A2 (Beta)](https://download.msi.com/bos_exe/mb/7C02v3A2.zip)

## Specifications
| **Component** | **Model** |
| ------------- | --------- |
| CPU | Ryzen 7 3700x |
| Motherboard | MSI B450 Tomahawk Max |
| GPU | XFX RX 5700 XT THICC III |
| RAM | 32GB 3200MHZ |
| OS Disk (SSD) | PNY CS3030 |
| LAN CHIPSET | Realtek® 8111H|
| AUDIO CHIPSET | Realtek® ALC892 |
| CASE | Corsair Corbide 270R |

## What works
 - Hardware accelerated Encode/Decode (Amazon / Netflix / Hulu)
 - Ethernet 
 - Audio  
 - CPU Power Management
 - GPU Power Management
 - FileVault
 - Sleep (macOS 11.0+)
 - iServices

 ## Issues
  - Partially-working virtualization (only VirtualBox & Parallels Dekstop 13.1.0 or below)
  - Not working 3.5mm Jack microphone (only USB/Bluetooth microphones)

## How to use
  1. [**Create bootable USB**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/).  
  2. Clone this repository, copy and paste "EFI" directory onto your USB drive.
  3. [**Set up SMBIOS (MacPro7,1) and MAC address**](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#generate-a-new-serial).  
  4. Set BIOS settings according to the [**guide**](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#amd-bios-settings).  
  5. [**Install macOS**](https://dortania.github.io/OpenCore-Install-Guide/installation/installation-process.html#booting-the-opencore-usb). 

## Other Guides
**If you have any problems with installation or booting your macOS, kernel panics or another system related issues check OC configuration guide**  
**If something else isn't working properly (for example USB ports, iServices, DRM/Netflix) check Post-Install guide**
 - [Post-Install](https://dortania.github.io/OpenCore-Post-Install/)
 - [Multiboot](https://dortania.github.io/OpenCore-Post-Install/#multiboot)
 - [Troubleshooting](https://dortania.github.io/OpenCore-Post-Install/)
 - [ACPI Patching](https://dortania.github.io/Getting-Started-With-ACPI/)
 - [USB Mapping](https://dortania.github.io/OpenCore-Post-Install/usb/)
 - [MacPro7,1 Memory Errors](https://dortania.github.io/OpenCore-Post-Install/universal/memory.html)

If you have any other questions or issues, feel free to ask on [**AMD-OSX Discord**](https://discord.gg/EfCYAJW) or [**Forum**](https://forum.amd-osx.com)  

## Credits
- [**acidanthera**](https://github.com/acidanthera) for [OpenCore](https://github.com/acidanthera/OpenCorePkg), [AppleALC](https://github.com/acidanthera/AppleALC), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [WhateverGreen](https://github.com/acidanthera/WhateverGreen),
    [NVMEFix](https://github.com/acidanthera/NVMeFix)
- [**AMD-OSX**](https://github.com/AMD-OSX) for [AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla) CPU patches
- [**Mieze**](https://github.com/Mieze) for [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [**trulyspinach**](https://github.com/trulyspinach) for [AMDRyzenCPUPowerManagement](https://github.com/trulyspinach/SMCAMDProcessor) and [SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)
- [**dortania**](https://github.com/dortania) for amazing [documentation](https://dortania.github.io/OpenCore-Install-Guide/)

