Modified from this guide here: http://blogs.wcode.org/2013/09/howto-boot-your-raspberry-pi-into-a-fullscreen-browser-kiosk/

Requires: matchbox firefox x11-xserver-utils ttf-mscorefonts-installer ttf-liberation xwit libnss3
(Use code below to install)

sudo apt-get update
sudo apt-get dist-upgrade
sudo apt-get install matchbox matchbox-window-manager firefox-esr x11-xserver-utils ttf-mscorefonts-installer ttf-liberation xwit libnss3
sudo reboot


- Place config.txt and xinitrc on the boot partition (/boot if the pi is running) and make sure it's owned by root.

- Copy the contents of rc.local into /etc/rc.local

- Reboot
