# Companion-Pi2
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/ardupilot_logo2.png)

This is a collection of Linux .img files & Software to allow drone users to hook up to a Raspberry Pi2 and further their drone experiences in various ways. It is designed to allow non-linux users to get up and running without having to run terminal commands etc. All software is provided as-is and you assume all risks by using it. 

# Project Goals:
I hope to create different .img files as I journey along which will allow users to perform different tasks depending upon which .img file they burn to their Micro SD card, insert into pi2, and boot. Simple!
- some version goals include:
- video and drone comms (V1.0)
- OpenCV (Object detection & Avoidance) (V2.0)
- Caffe (Object naming/identification) (V3.0)
- Lidar (Object detection & avoidance) (V4.0)

# Version 1.0 (All tested by me as working):
- Raspbian Jessie (based upon Debian v8?) operating system (others can be added when tested working)
- Gstreamer (For video transmission using pi camera)
- MavProxy/Mavlink/DroneCode (For APM/Pixhawk communication)

# Burning .img to SD Card:
We will use Win32Diskimager software on Windows, available here: https://sourceforge.net/projects/win32diskimager/

- open the software and we have this menu:

![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/Win32DiskImager.png)
- click the folder icon and select the pi2 .img file you have downloaded from this github repo
- select the correct sd card using the device tab
- click write, and wait for the progress bar to complete writing
- insert into your pi2 and boot/power on
- done!

- SD Card used by me is a Transcend 'Premium 400x' Micro SD 16GB. It is working fine with Raspbian Jessie and it is quicker than other cards I have around. It costs as low as £3.88 on amazon as of 25/04/2016.
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/sd16gb.jpg)


# USB wifi dongles used/tested (plug & play):
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/2016-04-24_001.jpg)
- Ralink RT5370: cheap $2 readily available dongle to get you up and testing
- (More added as I get through the ones I have, feel free to message me if yours working)


# Basic Hardware Connection:
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/pi2-connections.jpg)
- This is how to connect all the system parts to enable .img (V1.0) to send video and send/receive data to a device (Laptop/PC/Tablet)
- range is limited to the wifi connection range, so ensure you have enough range and also backup control using a normal RC radio controller to the APM/Pixhawk board

# Advanced Hardware Connection:
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/pi2-connections2.jpg)

# Software Connection:
- There are many ways to skin a cat, as they say. The various ways will be offered in time as I write how-to. 
- Basic methods include:

- Manually using SSH & commands (fiddly and annoying)
- Automatic 1-button-press connection (In development)
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/2016-04-24_002.jpg)
- - Using Mission Planner software & Video HUD on Windows Laptop
- - Using Android Tower Beta software on Android Tablet
- - Using Ubuntu & APM Planner software on Laptop (in beta)

More will be added/edited as progress is made. Please send me PM me if you have changes/updates or if you have made an .img file an blog to link to: email:i6mods@gmail.com RCgroups.com:Benbojangles Diydrones.com:Benbojangles Blog:http://dalybulge.blogspot.co.uk
