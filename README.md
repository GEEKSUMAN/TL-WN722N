# Monitor mode 
# Frame Injection
# aircrack-ng
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


βββ(rootπsherspect)-[~]
ββ# lsusb

βββ(rootπsherspect)-[~]
ββ# iwconfig

βββ(rootπsherspect)-[~]
ββ# sudo -i

βββ(rootπsherspect)-[~]
ββ# apt install realtek-rtl8188* -y  

βββ(rootπsherspect)-[~]
ββ# pwd

βββ(rootπsherspect)-[~]
ββ# echo "blacklist r8188eu.ko" βΊ "/etc/modprobe.d/realtek.conf"

βββ(rootπsherspect)-[~]
ββ# git clone https://github.com/aircrack-ng/rtl8188eus.git

βββ(rootπsherspect)-[~]
ββ# cd rtl8188eus

βββ(rootπsherspect)-[~]
ββ# make

βββ(rootπsherspect)-[~]
ββ# make install

βββ(rootπsherspect)-[~]
ββ# reboot

βββ(rootπsherspect)-[~]
ββ# ### check Tp-Link TL-WN722N WiFi Adapter is connected in virtual box ###

βββ(rootπsherspect)-[~]
ββ# airmon-ng check kill

βββ(rootπsherspect)-[~]
ββ# ifconfig wlan0 down

βββ(rootπsherspect)-[~]
ββ# iwconfig wlan0 mode  monitor 

βββ(rootπsherspect)-[~]
ββ# iwconfig

ππππππππππππππππππππππππππππππππππππππππππππππππππππππππππππ

### If you like it ; share my repo , it will be token of love for me <3 #####


