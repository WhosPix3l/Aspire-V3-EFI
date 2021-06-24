# Opencore EFI folder, for the Lenovo Yoga 2!

Tested on macOS Big Sur, but should work with older and newer versions of macOS.
Credits to **[@losowyLP](https://github.com/losowyLP)** for letting me Hackintosh his system!

:exclamation: Don't forget to generate a new SMBIOS with GenSMBios! (We're using MacBookPro11,4)

:exclamation: This EFI is a work in progress. Even though it boots, not everything has been tested.

## System Specifications

### CPU
* Intel Core i3-4030U @ 1.90 GHz (Two cores, four threads)
### Memory
* Unknown 8GB DDR3L 1600 MHz SODIMM
### Graphics
* Intel HD Graphics 4400
* 13.3" 1920 × 1080 (Full HD) multitouch display
### Connectivity
* Intel Dual-Band Wireless AC-7260
* Intel Bluetooth
### Ports
* 1 ✕ Combo jack (Input + Output)
* 1 ✕ Lenovo rectangle power connector
* 1 ✕ Micro HDMI port
* 1 ✕ SD card reader
* 1 ✕ USB 3.0
* 1 ✕ USB 2.0 (broken)
### Input
* PS/2 Keyboard + Trackpad
* WebCam


## Features


### Fully working
* All USB ports (can't test lol)
* Battery management
* Bluetooth
* Brightness control
* Built-in audio speakers
* Graphics acceleration with iGPU

### Somewhat working
* App Store
* Trackpad (Only scroll gestures work, enable 'Click in bottom right corner' to get right-click to work.)
* WiFi + Bluetooth (really slow)

### Not working
* Sleep + wake
* iServices (App Store, FaceTime, iMessage, etc.)
* WebCam (Haven't gotten around to USB mapping yet, will do soon however)

## BIOS Settings


* Boot → Boot Mode → Legacy
* Boot → Boot Mode → UEFI First
* Security → Secure Boot → Off
* Configuration → Intel Virtualization Technology → Enabled


## Changelog (DD/MM/YYYY)

### 24/06/2021
* Works now!

### 23/06/2021
* Tried another framebuffer

### 22/06/2021
* Made EFI
