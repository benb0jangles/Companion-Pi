# Companion-Pi
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/ardupilot_logo2.png)

This is a collection of Linux .img files & Software to allow drone users to hook up to a Raspberry Pi 2/3/Zero V1.2/1.3 and further their drone experiences in various ways. It is designed to allow non-linux users to get up and running without having to run terminal commands etc. All software is provided as-is and you assume all risks by using it. 

The project may be utilised for many forms of automated vehicle purposes and is created to help further open hardware and software use in all unmanned vehicles. 

# Tested and working with:
- Raspberry Pi 2 
- Pi 3 (must do uart fix: https://www.raspberrypi.org/forums/viewtopic.php?t=138223)
- Pi Zero V1.2 (no camera)
- Pi Zero V1.3 (must use APMpi_Jessie_Lite img v1.0)

# Project Goals:
I hope to create different .img files as I journey along which will allow users to perform different tasks depending upon which .img file they burn to their Micro SD card, insert into pi, and boot. Simple!
- some version goals include:
- video and drone comms (V1.0)
- Auto Pi-Photo triggering & GPS Geotagging (V2.0)
- OpenCV (Object detection & Avoidance) (V3.0)
- Caffe (Object naming/identification) (V4.0)
- Lidar (Object detection & avoidance) (V5.0)

# Bucket List (to do list):
- add UDT error correction to udp
- gps/photo geotagging python script
- power-on/shutdown hardware buttons for both units
- Auto connect script
- testing different wifi modules/dongle

# Bucket List (stretch goal):
- gamepad control??? 

# Version 1.0 (All tested by me as working):
- Raspbian Jessie (based upon Debian v8?) operating system (others can be added when tested working)
- Gstreamer (For video transmission using pi camera)
- MavProxy/Mavlink/DroneCode (For APM/Pixhawk communication)
- Drone Pi .img file: https://github.com/benb0jangles/Companion-Pi/tree/master/APMPi%20img%20files/V1_0
- Ground Pi .img file: --added here--

# Burning .img to SD Card:
We will use Win32Diskimager software on Windows, available here: https://sourceforge.net/projects/win32diskimager/

- open the software and we have this menu:

![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/Win32DiskImager.png)
- click the folder icon and select the pi .img file you have downloaded from this github repo
- select the correct sd card using the device tab
- click write, and wait for the progress bar to complete writing
- insert into your pi and boot/power on
- done!

- SD Card used by me is a Transcend 'Premium 400x' Micro SD 16GB. It is working fine with Raspbian Jessie and it is quicker than other cards I have around. It costs as low as £3.88 on amazon as of 25/04/2016.
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/sd16gb.jpg)
- I also am using 2gb (Openwrt, Raspbian Jessie Lite just fits with mavproxy & gstreamer-plugins-good), 4gb, 8gb micro sd cards for different .img file tests. Some sd cards work, some do not.


# USB wifi dongles used/tested (plug & play):
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/2016-04-24_001.jpg)
- Ralink RT5370: cheap $2 readily available dongle to get you up and testing
- RealTek RTL8188CUS: another cheap $2 dongle with external antenna
- (More added as I get through the ones I have, feel free to message me if yours working #check using 'lsusb' command in pi terminal or ssh terminal)
- List here: https://github.com/benb0jangles/Companion-Pi/tree/master/Wifi%20Dongle%20List


# Basic Hardware Connection:
![](https://github.com/benb0jangles/Companion-Pi/blob/master/Images%20for%20readme/2016-05-19_0022.jpg)
- This is how to connect all the system parts to enable .img (V1.0) to send video and send/receive data to a device (Laptop/PC/Tablet)
- range is limited to the wifi connection range, so ensure you have enough range and also backup control using a normal RC radio controller to the APM/Pixhawk board

# Software Connection:
- There are many ways to skin a cat, as they say. The various ways will be offered in time as I write how-to. 

- Manually using SSH & commands (fiddly and annoying)
- Automatic 1-button-press connection (In development)
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/2016-04-24_002.jpg)
- - Using Mission Planner software & Video HUD on Windows Laptop
- - Using Android Tower Beta software on Android Tablet
- - Using Ubuntu & APM Planner software on Laptop (in beta)
- - Using QTgstreamerHUD on Raspbian for hdmi fpv (in discussion)

# Ground Hardware:
- Options
![](https://github.com/benb0jangles/Companion-Pi/blob/master/Images%20for%20readme/2016-05-27_002.jpg)

More will be added/edited as progress is made. Contributors needed (please review project bucket list). Please send me PM me if you have changes/updates or if you have made an .img file an blog to link to: email:i6mods@gmail.com RCgroups.com:Benbojangles Diydrones.com:Benbojangles Blog:http://dalybulge.blogspot.co.uk

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.
