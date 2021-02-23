Web USB terminal emulator (well, without actual emulation :-)

This uses webusb/winusb to allow a webpage to become a terminal emulator for a cdc/acm serial port USB device!

Click "Connect" to select your cdc/acm serial port USB device and then enter commands in the command line!

Your cdc/acm serial port USB device must not be claimed by usbser.sys or you will get an access denied error.

You may need to edit the default endpoint numbers and vendor/product filter:

  const epin = 2;  // bulk endpoint from cdc/acm device
  const epout = 3;  // bulk endpoint to cdc/acm device
  {vendorId: 0x0403, productId: 0xa660}  // CpuStick with cdc/acm class/subclass 02/02 replaced with FF/00

Try it here: https://rtestardi.github.io/usbte/usbte.html