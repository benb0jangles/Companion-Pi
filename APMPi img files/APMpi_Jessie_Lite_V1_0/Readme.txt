# Download Link: <here>

# APMpi_Jessie_Lite_V1_0 - Tested on Pi Zero V1.3 - Also (probably) working for pi2/3 by Benbojangles (27/05/2016)
- This .img file is V1 of a project I am working on. It is available under creative Commons License.

- This .img file is a custom raspbian image created for the Raspberry pi, it includes:
- Raspbian Jessie Lite (version from 24/05/2016)
- Gstreamer
- Mavproxy
- SSH Enabled
- Pi Camera enabled
- Disabled O/S control of Serial port
- Custom config.txt for performance
- Static IP enabled

File fits on 8gb sd card, and has 70% free space. Also fits on larger sd card (you can expand filesystem if wish to)

# How to burn to SD card:
- 1)Burn .img to sd card using win32diskimager.exe
- 2)Boot pi Zero
- 3)Jessie Lite is Command Line, so you plug in monitor & keyboard to setup wifi for ssh
- 4)Connect to your wifi by typing in & then editing: sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
- 4)Guide here: https://thepihut.com/blogs/raspberry-pi-tutorials/83502916-how-to-setup-wifi-on-raspbian-jessie-lite
- 5)Input your wifi SSID & Password, then writeout file by <shift> + o, then exit by shift + x.
- 6)Check you IP, type: ifconfig. it should show as 192.168.1.3 (remember for ssh connection)  
- 7)Shutdown pi 2/3/Zero and unplug keyboard/mouse/screen, restart pi 2/3/Zero
- 8)SSH connect: 192.168.1.3 port:22 - username:pi password:raspberry 
- 9)run mavproxy & gstreamer with settings as you wish (or use my settings)


- I hope to add more features in future once the groundpi 2/3/Zero is complete, there will not be a need to setup IP.

- Thanks, suggestions/future .img versions to i6mods@gmail.com
