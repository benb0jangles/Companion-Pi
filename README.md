# Companion-Pi2
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/ardupilot_logo.png)

This is a collection of Linux .img files to allow drone users to hook up to a Raspberry Pi2 and further their drone experiences in various ways. All software is provided as-is and you assume all risks by using it. 

# Project Goals:
I hope to create different .img files as I journey along which will allow users to perform different tasks depending upon which .img file they burn to their Micro SD card, insert into pi2, and boot. Simple!

# Version 1.0 (All tested by me as working):
- Raspbian Jessie (based upon Debian v8?) operating system
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

# Connection to flight controller:
![](https://github.com/benb0jangles/Companion-Pi2/blob/master/Images%20for%20readme/RaspberryPi_Pixhawk_wiring1.jpg)
This is how you connect an APM/Pixhawk flight board to a Raspberrypi2. In the image it shows a pixhawk, but the wiring is the same for APM - Just connect to the telemetry port (Or USB port if you change the baud rate for it)
