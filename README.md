**macOS version**: 10.15.1 - 12.2

**OpenCore version**: [0.7.8](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.7.8)

**BIOS version**: [7C02v3B](https://download.msi.com/bos_exe/mb/7C02v3B.zip)

## Specifications
| **Component** | **Model** |
| ------------- | --------- |
| CPU | Ryzen 7 3700x |
| Motherboard | MSI B450 Tomahawk Max |
| GPU | XFX RX 5700 XT Thicc III |
| RAM | 2x16GB 3200Mhz |
| OS Disk (SSD) | PNY CS3030 NVME |
| LAN CHIPSET | RTL8111H |
| AUDIO CHIPSET | ALC892 |

## What works
 - Hardware Acceleration
 - Ethernet 
 - Audio
 - USB Ports
 - CPU Power Management
 - FileVault
 - Sleep (macOS 11.0+)
 - iServices

 ## Issues
  - Partially-working virtualization (only VirtualBox & Parallels Dekstop 13.1.0 or below)
  - Not working 3.5mm Jack microphone (works with VoodooHDA, though the audio quality is noticeably worse)

## How to use

  1. [**Create bootable USB**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/).  
  2. Clone this repository, drag and drop the "EFI" directory onto your USB drive.
  3. [**Set SMBIOS for MacPro7,1**](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#generate-a-new-serial) and [**fix ROM**](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#fixing-rom).  
  4. Set BIOS settings according to the [**guide**](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#amd-bios-settings).  
  5. [**Install macOS**](https://dortania.github.io/OpenCore-Install-Guide/installation/installation-process.html#booting-the-opencore-usb).

## Other Guides

In case you are experiencing issues during installation or boot, kernel panics or other system related issues — check OC configuration guides:

 - [**Post-Install**](https://dortania.github.io/OpenCore-Post-Install/)
 - [**Troubleshooting**](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/troubleshooting.html)
 - [**OpenCore and Monterey**](https://dortania.github.io/OpenCore-Install-Guide/extras/monterey.html)
 - [**OpenCore and Big Sur**](https://dortania.github.io/OpenCore-Install-Guide/extras/big-sur/)
 - [**USB Mapping**](https://dortania.github.io/OpenCore-Post-Install/usb/manual/manual.html#usb-mapping-the-manual-way)
 - [**ACPI Patching**](https://dortania.github.io/Getting-Started-With-ACPI/)

If you have any other questions or issues, feel free to ask on [**AMD-OSX Discord**](https://discord.gg/EfCYAJW) or [**Forum**](https://forum.amd-osx.com)  

## Fix Application Crashes

- [**Adobe Products**](https://gist.github.com/naveenkrdy/26760ac5135deed6d0bb8902f6ceb6bd)
- [**Discord**](https://gist.github.com/bakedpotato191/ff82485e809594ab94c10abc26fa4121#file-discordamdfix-md)

## Credits
- [**acidanthera**](https://github.com/acidanthera) for [OpenCore](https://github.com/acidanthera/OpenCorePkg), [AppleALC](https://github.com/acidanthera/AppleALC), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [WhateverGreen](https://github.com/acidanthera/WhateverGreen),
    [NVMEFix](https://github.com/acidanthera/NVMeFix)
- [**AMD-OSX**](https://github.com/AMD-OSX) for [AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla) CPU patches
- [**Mieze**](https://github.com/Mieze) for [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [**trulyspinach**](https://github.com/trulyspinach) for [AMDRyzenCPUPowerManagement](https://github.com/trulyspinach/SMCAMDProcessor) and [SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)
- [**dortania**](https://github.com/dortania) for amazing [documentation](https://dortania.github.io/OpenCore-Install-Guide/)

