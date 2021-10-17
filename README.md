# kali linux touchpad not working problem solved

most of the cases that you don't have drivers for the touchpad on your laptop

this how i solved my problem:

```
# apt-cache search touchpad

libevdev-tools - wrapper library for evdev devices - tools
libspandsp-dev - Telephony signal processing library - development headers
libspandsp-doc - Documentation for the spandsp signal processing library
libspandsp2 - Telephony signal processing library
libukui-touchpadclient-dev - touchpad settings interfaces
libukui-touchpadclient0 - touchpad settings module
olpc-kbdshim - OLPC XO keyboard support daemon
ukui-touchpadserver - touchpad settings service process
xserver-xorg-input-libinput - X.Org X server -- libinput input driver
xserver-xorg-input-mtrack - Multitouch X input driver
xserver-xorg-input-multitouch - Multitouch X input driver
xserver-xorg-input-synaptics - Synaptics TouchPad driver for X.Org server
xserver-xorg-input-synaptics-dev - Synaptics TouchPad driver for X.Org server (development headers)
```
```
# apt install xserver-xorg-input-libinput  xserver-xorg-input-multitouch xserver-xorg-input-synaptics xserver-xorg-input-synaptics-dev

# apt install xserver-xorg-input-mtrack

$ reboot
```


