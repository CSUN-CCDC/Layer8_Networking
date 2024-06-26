Here is what worked worked, while all other suggestions on the internet did not:

apk add udev xf86-input-libinput

rc-update add udev-trigger boot
rc-update add udev-settle boot
rc-update add udev-postmount boot

reboot
