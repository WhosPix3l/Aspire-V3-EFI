# Opencore EFI folder, for the Acer Aspire V3-371!

Tested on macOS Catalina, but should work with older versions of macOS.

:exclamation: Don't forget to generate a new SMBIOS with GenSMBios! (I'm using MacBookPro11,1)

:exclamation: This EFI is a work in progress. Even though it boots, not everything has been tested.

## System Specifications


##### Laptop:
* Acer Aspire V3-371
##### Motherboard:
* Acer Aspire V3-371
##### CPU:
* Intel Core i3-4005U
##### Memory:
* Crucial 8GB DDR3L 1600 MHz SODIMM
* Generic 4GB DDR3L 1600 MHz SODIMM (Comes with the laptop configuration)
##### Graphics:
* Intel HD Graphics 4400
##### Networking:
* Intel Dual-Band Wireless AC-7265
* Realtek Ethernet RTL8111
##### Connectivity:
* 1 ✕ Barrel power connector
* 1 ✕ Ethernet port
* 1 ✕ HDMI port
* 1 ✕ USB 3.0
* 1 ✕ USB 2.0
* 1 ✕ SD card reader
* 1 ✕ Combo jack (Input + Output)


## Features


##### What's working:
* Adjustable display backlight
* All USB ports
* Battery management
* Built-in keyboard
* Gigabit Ethernet
* Graphics acceleration with iGPU
* Intel Bluetooth
* WebCam

##### What's somewhat working:
* App Store
* iCloud
* Logging in with an Apple ID on the Hackintosh
* Touchpad (Only scroll gestures work, enable 'Click in bottom right corner' to get right-click to work.)

##### What's not working:
* Built-in audio (Will try with VoodooHDA later)
* Built-in WiFi
* HDMI port (Haven't got around to do BusID patching)
* Rest of the iServices (FaceTime, iMessage, etc.)
* Sleep + wake

## BIOS Settings


* Boot → Boot Mode → UEFI
* Boot → Secure Boot → Disable


## Changelog (DD/MM/YYYY)


### 01/10/2020
* Moved SystemProfilerMemoryFixup.kext to the Extensions folder as macOS kernel panics when trying to boot into Recovery.

### 27/09/2020
* Add SystemProfilerMemoryFixup.kext in order to show the memory tab in the 'About This Mac' window.
* Initial commit.