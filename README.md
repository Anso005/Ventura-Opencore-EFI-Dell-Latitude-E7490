 IT IS IMPORTANT TO READ THE DESCRIPTION BEFORE INSTALLING
# Dell Latitude 7490 Hackintosh EFI
# MacOS 11.x Ventura via Helliport=For Internet Module

## History
This project is all alone developed by me. I took me 11 months to make the efi.
I have been using this hackintosh for a long time, and it works well on my laptop.
Every think works flawlessly.
You can show your support by sponsoring me. It will indeed be a sign of appreciation.

Note: This efi is made on basis of Dell latitude e7490. This can also be used with similar spec Dell laptop.

## IMPORTANT NOTE (VERY IMPORTANT AT BOOTING PROCESS AFTER MacOS IS INSTALLED)
Note: When laptop is turned on don't press any keyboard key or button. At Apple logo when the loading bar is at half press Fn+PrtSCR(located next to F12 key).
This will turn off wlan driver. If not pressed the laptop will stay stuck at the half loading bar.
After pressed the screen will blink and loading will be completed. You will be directed to login page of MacOs

## Tested macOS version:
macOS 13.5-13.5.1 using OpenCore 0.6+

## Intsallation Process:
For installation process I recommend watching this youtube video: https://www.youtube.com/watch?v=J1d0AmVFWKM. He uses EFi for pc. You need to download the one for laptop. As, my laptop has coffelake processor, so I used opencore efi for coffeelake laptop. I have uploaded it with name EFI(BOOTING). But note that when placing it on usb rename it to EFI. After the macos has been installed according to video place efi named EFI(MAIN) in the MacOs boot drive and rename it back to EFI. All steps are explained in the video. Just use my files instead of those used in his video.


## System configuration
- Intel Core i5-8350U
- 8GB DDR4-2400MHz RAM 8gb(can also be used with other configuration of ram i.e 16gb or 32gb etc)
- Intel UHD 620 Graphics
- Samsung SSD 970 EVO 256gb(can also be used with other configuration of storage i.e 500gb, 1000gb etc)
- Intel Dual-Band Wireless-AC 8265
  #### Note:
  To use internet you need to install Helliport.dmg in your system and add it in login items.
  Download it from official repository: https://github.com/OpenIntelWireless/HeliPort/releases/tag/v1.4.1

## Confirm working
1) Loudspeaker
2) 3.5mm headphone jack^
4) Battery Management
5) Backlight Control (Fn+B & Fn+S or Fn+F11 & Fn+F12)
6) Ethernet
7) Touchpad with Gestures and buttons
8) WiFi (2.4/5GHz) via Helliport)
Note: Airportwlm can also be used for as internet kext but is buggy sometimes. I recommend Helliport.
9) Bluetooth Audio*
10) USB-C Power Delivery for Charging (Apple 61W, Ugreen 65W)
11) Barrel Plug for Charging (Dell 90W)
12) FileVault
13) CPU SpeedStep
14) iGPU Acceleration
15) Native hotkey support with Fn keys
16) Dual-booting with Windows (Native dual-boot, not through BootCamp / Parallels)
17) HDMI output
18) SideCar using USB-A to lightning _(tested on iPad 7th/9th generation, WiFi+Cellular)_
19) Trackpoint and all trackpad keys are working smoothly.
^_3.5mm headphone jack might not work properly after system wakes from sleep, intalling codec commander will resolve this issue._

## Not working
The only thing which doesn't potentially work is docking moniters by thunderbolt 3.
It's a common issue in hackintosh.
But charging via thunderbolt+Usb-C port works flawlessly.

## Resolving Sleep Isue
After installing MacOs sucessfully. The first issue you will be facing which I faced is sleep and shutdown issue.
I resolved it by opening the back lid and disconnecting the laptops battery. Then unplug CMOS battery. Press and hold down power button of laptp for 1 minute. This will be reseting the laptops bios and settings. After holding the power button for 1 minute re-attach the CMOS and laptops battery. Close the lid. Turn on the laptop and your sleep and shutdown issue will be resolved.
All steps can be seen in this video: https://www.youtube.com/watch?v=kTYlxcL1cQc
### Note:
This has been tested by me. I have been using this alptop for over 6 months now with bigsur, then montery and now ventura. No sleeping issues were seen afterwards. But if you clen install MacOs again via usb. You will need to repeat the steps above.

### Method for logging in to Apple ID
Use GenBios to generate Serial, ID and MLB for your machine.
Follow this tutorial: https://www.youtube.com/watch?v=TWMZb_fu2hk
Afterwards, simply login your Apple ID.

## More To come:
I will be demostrating all these processes via youtube. I just need support for you. Together we will create a community and help other users learn the art of hackintoshing.
Support me by sponsoring or paying me as an appreciation. 
I will also me helping my sponsors by talking to them on calls.

## Thank You For Your Love & Support.
