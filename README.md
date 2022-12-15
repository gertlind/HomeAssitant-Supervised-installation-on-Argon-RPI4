# HomeAssistant
## Supervised installation on Argon RPI4
### Install Pi OS
[https://www.raspberrypi.com/software/](url)
- Insert the MicroSD in the Raspberry and start.
	- Log in and update below.
```
sudo apt update
sudo apt full-upgrade
sudo rpi-update
sudo reboot
sudo rpi-eeprom-update -d -a
```
### Make below settings in raspi-config

- raspi-config
	- Advanced Options
		- Bootloader Version
			- [Boot ROM Version]
				- [Latest Use the latest version boot ROM software]
					- [Reset to Default] - [No]
					- [Boot ROM not reset to defaults] - [Ok]
			- Advanced Options
				- [Boot Order]
					- [USB Boot]
						- [USB device is default boot device] - [Ok]
		- [Finish]
		- [Would you like to reboot now] - [Yes]

### Install git
```
sudo apt-get install git
```

### Install Argon tool

[https://www.waveshare.com/wiki/PI4-CASE-ARGON-ONE](url)
```
curl https://download.argon40.com/argon1.sh | bash
```
```
settings
argonone-config 
```
### Install Home Assistant Supervised
https://community.home-assistant.io/t/guide-how-to-install-home-assistant-supervised-on-rpi4-with-raspios-64-bit-october-2022/480855
### Install HACS
https://www.wundertech.net/how-to-install-hacs-on-home-assistant/<br>
### Install rpi-clone
[https://github.com/billw2/rpi-clone](url)<br>
```
git clone https://github.com/billw2/rpi-clone.git
sudo cp rpi-clone/rpi-clone rpi-clone/rpi-clone-setup /usr/local/sbin
```
Clone the memory card to the SSD disk:<br>
 ```sudo rpi-clone -f -p 240M sda```<br>
<i>This takes a while......</i><br>


