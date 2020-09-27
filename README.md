# Opencore EFI folder, for the Acer Aspire V3-371!

Tested on macOS Catalina, but should work with older versions of macOS.

:exclamation: Don't forget to generate a new SMBIOS with GenSMBios! (I'm using MacBookPro11,1)

:exclamation: This EFI is a work in progress. Even though it boots, not everything has been tested.

##### What's working:
* Adjustable display backlight
* All USB ports
* Battery management
* Gigabit Ethernet
* Graphics acceleration with iGPU (Intel HD Graphics 4400)
* Built-in keyboard
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

##### BIOS Settings
* Boot → Boot Mode → UEFI
* Boot → Secure Boot → Disable

## Changelog

## &#x1F34F;   Initial commit.