# victron-automationhat
Adds support to Victron Venus OS (on Raspberry Pi) for Pimoroni AutomationHat

# Pre-Requirements

Edit /u-boot/config.txt and add the following line:

  dtparam=i2c_arm=on

Add the following line to /data/rc.local:

  modprobe i2c-dev
  
