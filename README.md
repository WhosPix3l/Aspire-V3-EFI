# Opencore EFI folder, for the Acer Aspire V3-371!

Tested on macOS Big Sur, but should work with older and newer versions of macOS.

:exclamation: Don't forget to generate a new SMBIOS with GenSMBios! (I'm using MacBookPro11,1)

:exclamation: This EFI is a work in progress. Even though it boots, not everything has been tested.

## System Specifications

### CPU
* Intel Core i3-4005U @ 1.70 GHz (Two cores, four threads)
### Memory
* Corsair ValueSelect 8GB DDR3L 1600 MHz SODIMM
* Samsung 4GB DDR3L 1600 MHz SODIMM (Comes with the laptop configuration)
### Graphics
* Intel HD Graphics 4400
### Connectivity
* Intel Dual-Band Wireless AC-7265
* Intel Bluetooth
* Realtek Ethernet RTL8111
### Ports
* 1 ✕ Barrel power connector
* 1 ✕ Ethernet port
* 1 ✕ HDMI port
* 1 ✕ USB 3.0
* 1 ✕ USB 2.0
* 1 ✕ SD card reader
* 1 ✕ Combo jack (Input + Output)
### Input
* PS/2 Keyboard
* Synaptics I2C Trackpad
* (Chicony?) HD WebCam


## Features


### Fully working
* All USB ports
* App Store
* Battery management
* Brightness Control
* Built-in audio speakers
* Built-in keyboard
* Gigabit Ethernet
* Graphics acceleration with iGPU
* HDMI port (Finder will crash and you must hard reset.)
* iServices (App Store, FaceTime, iMessage, etc.)
* WiFi + Bluetooth

### Somewhat working
* Bluetooth
* Trackpad (Only scroll gestures work, enable 'Click in bottom right corner' to get right-click to work.)
### Not working
* Sleep + wake
* WebCam (Haven't gotten around to USB mapping yet, will do soon however)

## BIOS Settings


* Boot → Boot Mode → UEFI
* Boot → Secure Boot → Disable


## Changelog (DD/MM/YYYY)

### 03/06/2021
* Bump OC version OpenCore version 0.7.0
* Change SMBIOS to MacBookPro11,4

### 31/12/2020
* Add GUI
* Bump OC version to OpenCore version 0.6.4
* Cheers to a new year! 🥂

### 09/10/2020
* Attempted BusID patching, failed. Rolled back changes.

### 01/10/2020
* Removed SystemProfilerMemoryFixup.kext as macOS kernel panics when trying to boot into Recovery.

### 27/09/2020
* Add SystemProfilerMemoryFixup.kext in order to show the memory tab in the 'About This Mac' window.
* Initial commit.
