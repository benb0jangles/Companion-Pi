# Companion-Pi
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/ardupilot_logo2.png)

This is a collection of Linux .img files & Software to allow drone users to hook up to a Raspberry Pi Zero V1.3 and send/receive low latency Video + Mavlink Telemetry from drone-to-goggles. All software is provided as-is and you assume all risks by using it. 

The project may be utilised for many forms of automated vehicle purposes (drone/plane/rover) and is created to help further open hardware and software use in all unmanned vehicles. 

# Tested and working with:
- Pi Zero V1.3

# Project Goals:
I hope to create different .img files as I journey along which will allow users to perform different tasks depending upon which .img file they burn to their Micro SD card, insert into pi, and boot. Simple!
- some version goals include:
- video and drone comms (V1)
- Auto Pi-Photo triggering & GPS Geotagging (V2)
- OpenCV (Object detection & Avoidance) (V3)
- Caffe (Object naming/identification) (V4)
- Lidar (Object detection & avoidance) (V5)

# Bucket List (to do list):
- add UDT error correction to udp
- gps/photo geotagging python script
- power-on/shutdown hardware buttons for both units
- Auto connect script
- testing different wifi modules/dongle

# Bucket List (stretch goal):
- gamepad control??? 

# Version 1.1 (in progress, hey i'm a one man dev team :) ):
- Raspbian Jessie Lite
- Gstreamer (For video transmission using pi camera)
- MavProxy/Mavlink/DroneCode (For APM/Pixhawk communication)
- Drone Pi .img file: https://drive.google.com/open?id=0B1cVb3uX0f0dQTZzSmVISFdYd3M
- Goggles Pi .img file: https://drive.google.com/open?id=0B1cVb3uX0f0dakFpaTAyVF9HV2s
- Ground Module Pi .img file: --added here when ready--

# Burning .img to SD Card:
Use Win32Diskimager software on Windows, available here: https://sourceforge.net/projects/win32diskimager/

- open the software and we have this menu:

![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/Win32DiskImager.png)
- click the folder icon and select the pi .img file you have downloaded from this github repo
- select the correct sd card using the device tab
- click write, and wait for the progress bar to complete writing
- insert into your pi and boot/power on
- done!

- SD Card used by me is a no-brand 2GB card. It is working fine with Raspbian Jessie Lite.


# USB wifi dongles used/tested (plug & play):
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/2016-04-24_001.jpg)
- Ralink RT5370: cheap $2 readily available dongle to get you up and testing
- RealTek RTL8188CUS: another cheap $2 dongle with external antenna
- (More added as I get through the ones I have, feel free to message me if yours working #check using 'lsusb' command in pi terminal or ssh terminal)
- List here: https://github.com/benb0jangles/Companion-Pi/tree/master/Wifi%20Dongle%20List

# Equipment Costs - If you are interested in this project and want to pick it up, here is a brief list of parts and costs I use
- Pi Zero V1.3 (with camera port) £4.50 each
- USB wifi dongle £1 each
- Pi 2 £15 (on ebay)
- micro SD cards (from) £1.50
- pi camera £10
- pi camera ribbon cable £2
- Pi zero DIY USB Hub £1 (pound store)
- 3D Printed cases (free as I have a printer)
- Optional parts: U.fl antenna adapters, U.fl antennas, push-to-make switches, pin header wires, usb power, hdmi lead.

# Basic Hardware Connection:
![](https://github.com/benb0jangles/Companion-Pi/blob/master/Images%20for%20readme/2016-05-19_0022.jpg)
- This is how to connect all the system parts to enable .img (V1.0) to send video and send/receive data to a device (Laptop/PC/Tablet)
- range is limited to the wifi connection range, so ensure you have enough range and also backup control using a normal RC radio controller to the APM/Pixhawk board
 

# Ground Hardware:
- Options
![](https://github.com/benb0jangles/Companion-Pi/blob/master/Images%20for%20readme/2016-05-27_002.jpg)

More will be added/edited as progress is made. Contributors needed (please review project bucket list). Please send me PM me if you have changes/updates or if you have made an .img file an blog to link to: email:i6mods@gmail.com RCgroups.com:Benbojangles Diydrones.com:Benbojangles Blog:http://dalybulge.blogspot.co.uk

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.
