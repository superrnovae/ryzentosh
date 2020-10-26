![Screenshot](/cover.png?raw=true)

**macOS Catalina**: 10.15.7

**OpenCore version**: 0.6.2

## Specification
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 7 3700x @ 3.6GHz |
| Motherboard | MSI B450 TOMAHAWK MAX |
| GPU | AMD RX 5700 XT |
| RAM | 32GB GSkill Ripjaws V @ 3200MHz |
| OS Disk (SSD) | PNY CS3030 500GB |

### Software
1. [gibMacOS](https://github.com/corpnewt/gibMacOS)
2. [SSDT Time](https://github.com/corpnewt/SSDTTime)
3. [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
4. [Kexts Repository](https://github.com/acidanthera/bugtracker/) 
5. [ProperTree](https://github.com/corpnewt/ProperTree)

### Patches & Kexts
- [Lilu](https://github.com/acidanthera/VirtualSMC/releases) [Kext]   
- [VirtualSMC](https://github.com/acidanthera/VirtualSMC/releases) [Kext]   
- [AppleALC](https://github.com/acidanthera/AppleALC/releases) [Kext]   
- [AppleMCEReportedDisabler](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip) [Kext]   
- [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases) [Kext]   
- [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases) [Kext]   
- [USBMap](https://github.com/corpnewt/USBMap) [Kext]   
- [AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla/blob/opencore/17h/patches.plist) [Patch]   

## Functionality
### What works
- Hardware accelerated Encode/Decode (Amazon / Netflix / Hulu)   
- Audio   
- USB   
- Photoshop   
- AppStore   

###What doesn't work
- iMessage / FaceTime / iCloud (valid SN required)   
### Untested

### Untested
- Sleep    
- FileVault   

## Installation
  1. Create a macOS bootable usb with [gibMacOS](https://github.com/corpnewt/gibMacOS)
  2. Clone this repo and replace directiories "BOOT" and "OC" with the clonned ones.
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select config.plist from the /EFI/OC directory to automatically populate the fields.
  4. Alternativelly one could open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB  (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.
  5. Enjoy your Hackintosh ;)
