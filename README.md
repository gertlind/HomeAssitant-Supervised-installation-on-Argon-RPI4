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
### Install git
```
sudo apt-get install git
```
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
https://www.wundertech.net/how-to-install-hacs-on-home-assistant/
### Install rpi-clone
[https://github.com/billw2/rpi-clone](url)
```
git clone https://github.com/billw2/rpi-clone.git
cd rpi-clone
sudo cp rpi-clone rpi-clone-setup /usr/local/sbin<br>
Clone the memory card to the SSD disk: ```sudo rpi-clone -f -p 240M sda```<br>
<i>This takes a while......</i><br>


