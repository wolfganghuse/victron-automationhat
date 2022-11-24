# victron-automationhat
Adds support to Victron Venus OS (on Raspberry Pi) for Pimoroni AutomationHat

# Pre-Requirements

Edit /u-boot/config.txt and add the following line:

  dtparam=i2c_arm=on

Add the following line to /data/rc.local:

  modprobe i2c-dev
  
Update Packages

  opkg update && opkg install gcc make pkgconfig binutils python3-pip python3-spidev python3-dev

Create symlink for cc (not needed for Large Image)

  ln -s /usr/bin/arm-ve-linux-gnueabi-gcc /usr/bin/cc
  
Install AutomationHat Library

  pip3 install AutomationHat
  
