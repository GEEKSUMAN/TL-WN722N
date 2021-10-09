Monitor mode Frame Injection MESH Mode 
Android aircrack-ng
# TL-WN722N
TP-Link Nano USB WiFi Dongle 150Mbps High Gain Wireless Network Wi-Fi Adapter setting up for Kali Linux .
Its support monitor mood and packet sniffing, injection in V3/V2 realtek chipset.
Just follow bellow steps.

### Make sure your apt packages are uptodate of kali linux.

### Go to virtual box device settings options 
   >> Go to usb settings 
   >> 
   >> Add usb filters of the tplink adapter Realtek 802.11n NIC
   >> 
   >> Go to usb filters setings of Realtek 802.11n NIC
   >> 
   >> Clear all field except Name, Vendor ID , Product ID
   >> 
   >> save 
### Check if Kali is showing available wifi networks then all ok


┌──(root💀sherspect)-[~]
└─# lsusb

┌──(root💀sherspect)-[~]
└─# iwconfig

┌──(root💀sherspect)-[~]
└─# sudo -i

┌──(root💀sherspect)-[~]
└─# apt install realtek-rtl8188* -y  

┌──(root💀sherspect)-[~]
└─# pwd

┌──(root💀sherspect)-[~]
└─# echo "blacklist r8188eu.ko" › "/etc/modprobe.d/realtek.conf"

┌──(root💀sherspect)-[~]
└─# git clone https://github.com/aircrack-ng/rtl8188eus.git

┌──(root💀sherspect)-[~]
└─# cd rtl8188eus

┌──(root💀sherspect)-[~]
└─# make

┌──(root💀sherspect)-[~]
└─# make install

┌──(root💀sherspect)-[~]
└─# reboot

┌──(root💀sherspect)-[~]
└─# ### check Tp-Link TL-WN722N WiFi Adapter is connected in virtual box ###

┌──(root💀sherspect)-[~]
└─# airmon-ng check kill

┌──(root💀sherspect)-[~]
└─# ifconfig wlan0 down

┌──(root💀sherspect)-[~]
└─# iwconfig wlan0 mode  monitor 

┌──(root💀sherspect)-[~]
└─# iwconfig

💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀💀

### If you like it ; share my repo , it will be token of love for me <3 #####


