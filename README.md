# Hackintosh AMD for IOS Development 

[![MacOS version](https://img.shields.io/badge/Monterey-12.4-informational.svg)](https://www.apple.com/macos)\
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.8.0-informational.svg)](https://github.com/acidanthera/OpenCorePkg)

![MAC](https://user-images.githubusercontent.com/37451620/168442903-ad89265e-31ef-4132-87f5-b8e59844c9e0.png)

## OS Support and Tests
This EFI supports and was tested using MacOS versions:

* High Sierra.
* Monterey.

It can also supports other versions, but was not tested.

## Specification

| Component        | Model                                              |
| ---------------- | ---------------------------------------------------|
| CPU              | AMD Ryzen™ 5 2400G                                 |
| MotherBoard      | GA-A320M-S2H                                       |
| Wifi             | USB IWA 3000                                       |
| OS Disk          | SSD SATA A400 256gb                                |
| Other Disk       | Seagate ST2000DM008                                |
| RAM              | 2x 8gb Corsair Vengeance (16GB total)              |
| GPU              | Radeon™ RX 590 8GB                                 |

## Working

* iCloud
* Ethernet
* Wifi
* iServices
* Xcode 13.x
* IOS Simulation
* Virtualization

## Patches, Drivers & Kexts

* [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup)
* [HoRNDIS](https://github.com/jwise/HoRNDIS)
* [AppleALC](https://github.com/acidanthera/AppleALC)
* [USBMap](https://github.com/corpnewt/USBMap)
* [AppleMCEReporterDisabler](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)
* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla)
* [Lilu](https://github.com/acidanthera/Lilu)
* [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen)

## Bootloader

Able to dual-boot (Win11/Win10 + MacOS) but they need to be in separeted HDs

* MacOS: SSD SATA A400
* Windows: Seagate ST2000DM008 

## First Steps
* Install Python and 7zip (or WinRar)
* Download a RAW MacOS file (MacOSmonterey.raw)
* Use [Rufus](https://rufus.ie/) for creating the bootable device
* Open [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) select the second option and select the config.plist file
* On GenSMBIOS generate the Keys for MAC on options 3, 4 and 5
* Open [ProperTree](https://github.com/corpnewt/ProperTree) and on File options, select Clean Snapshot, than selct the file location folder
* After this use the pendrive to boot, Install MACOS
* After installing download Clover Bootloader to create a EFI Partition on your HardDrive
* Just copy the EFI folder from your pendrive to the EFI partition 

## Credits and links

* [OpenCore install guide](https://dortania.github.io/OpenCore-Install-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher)
* [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher)
* [OpenCore-Legacy-Patcher guide](https://dortania.github.io/OpenCore-Legacy-Patcher)

