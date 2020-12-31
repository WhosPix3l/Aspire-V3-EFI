# Opencore EFI folder, for the Acer Aspire V3-371!

Tested on macOS Mojave, but should work with older and newer versions of macOS.

:exclamation: Don't forget to generate a new SMBIOS with GenSMBios! (I'm using MacBookAir6,2)

:exclamation: This EFI does NOT inject SMBIOS to other operating systems in order to keep drivers working.

:exclamation: This EFI is a work in progress. Even though it boots, not everything has been tested.

## System Specifications


### Motherboard:
* Acer Aspire V3-371
### CPU:
* Intel Core i3-4005U
### Memory:
* Corsair ValueSelect 8GB DDR3L 1600 MHz SODIMM
* Samsung 4GB DDR3L 1600 MHz SODIMM (Comes with the laptop configuration)
### Graphics:
* Intel HD Graphics 4400
### Connectivity:
* Intel Dual-Band Wireless AC-7265
* Intel Bluetooth
* Realtek Ethernet RTL8111
### Ports:
* 1 ✕ Barrel power connector
* 1 ✕ Ethernet port
* 1 ✕ HDMI port
* 1 ✕ USB 3.0
* 1 ✕ USB 2.0
* 1 ✕ SD card reader
* 1 ✕ Combo jack (Input + Output)
### Input:
* PS/2 Keyboard
* Synaptics I2C Trackpad (Uses Microsoft drivers)
* (Chicony?) HD WebCam


## Features


##### What's working:
* All USB ports
* Battery management
* Bluetooth (natively!!)
* Built-in keyboard
* Gigabit Ethernet
* Graphics acceleration with iGPU

##### What's somewhat working:
* Adjustable display backlight (sometimes, not consistent)
* App Store
* HDMI port (Finder will crash and you must hard reset.)
* iCloud
* Logging in with an Apple ID on the Hackintosh
* Touchpad (Only scroll gestures work, enable 'Click in bottom right corner' to get right-click to work.)
* WebCam (sometimes, not consistent)

##### What's not working:
* Built-in audio (Still attempting a fix)
* Built-in WiFi
* Rest of the iServices (FaceTime, iMessage, etc.)
* Sleep + wake

## BIOS Settings


* Boot → Boot Mode → UEFI
* Boot → Secure Boot → Disable


## Changelog (DD/MM/YYYY)


### 31/12/2020
* Add GUI
* Bump OC version to OpenCore version 1.6.4
* Cheers to a new year! 🥂

### 09/10/2020
* Attempted BusID patching, failed. Rolled back changes.

### 01/10/2020
* Removed SystemProfilerMemoryFixup.kext as macOS kernel panics when trying to boot into Recovery.

### 27/09/2020
* Add SystemProfilerMemoryFixup.kext in order to show the memory tab in the 'About This Mac' window.
* Initial commit.
