# Opencore EFI folder, for [anthonyhfm](https://github.com/anthonyhfm)'s Ryzen build!

Tested on macOS Big Sur, but should work with older and newer versions of macOS.
Credits to **[@anthonyhfm](https://github.com/anthonyhfm)** for letting me Hackintosh his system!

:exclamation: Don't forget to generate a new SMBIOS with GenSMBios! (We're using iMac11,1)

:exclamation: This EFI is a work in progress. Even though it boots, not everything has been tested.

## System Specifications

### Motherboard
* Asus Prime B450 Plus
### CPU
* AMD Ryzen 5 3600 (6 cores, 12 threads)
### Memory
* 16 GB DDR4 3200 Mhz
### Graphics
* AMD Radeon RX 5600 XT


## Features


### Fully working
* All USB ports
* Graphics acceleration with GPU

### Somewhat working
* App Store

### Not working
* Sleep + wake
* iServices (App Store, FaceTime, iMessage, etc.)

## BIOS Settings

* Boot → Fast Boot → Disabled
* Boot → Secure Boot → Disabled
* Boot → CSM → Disabled
* Configuration → EHCI/XHCI Hand-off → Enabled
* Configuration → SATA Mode → AHCI


## Changelog (DD/MM/YYYY)

### 04/06/2021
* Made EFI
