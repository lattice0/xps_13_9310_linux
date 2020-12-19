# Dell XPS 13 9310 Linux 
This repo is a place for people to post issues about Linux (any distro) on Dell XPS 13 9310. I mainly work with Ubuntu so I'll share my experience below.

Currently, my issues are: couldn't install ubuntu 20.10 because of some disk error in the installation process (it installed once but never again), so I installed 20.04. The kernel that comes with it won't make touchscreen and sleep work, so I upgraded to 5.8, but 5.10 also worked fine.

For making bluetoth work on Ubuntu 20.04, I did https://askubuntu.com/questions/1299154/dell-xps-13-9310-bluetooth-wont-find-anything?noredirect=1#comment2210408_1299154, that is, you only have to download 2 firmware files and reboot. I thought it only worked with 5.8 but it works on 5.10. Ubuntu 20.10 should have those files already and thus work without any efforts but I have not tested it.

Wifi is still in development, you can follow here: https://github.com/kvalo/ath11k-firmware/issues/4. I think it can be made to work already but I did not try. I'm currently using my phone as a USB tether to share the wifi connection. XPS 13 9310 uses a different Wifi card than XPS 13 9300, which does not yet have a linux wifi driver (as of 19/12/2020).

Summary: On kernel 5.8 or 5.10 on Ubuntu 20.04, everything works except for wifi. Even touchscreen and sleep works. I do not have hopes for the fingerprint unlocking to work, I don't even know if Ubuntu has support for it, but it apears as a USB device on `lsusb`.


Feel free to open an issue.
