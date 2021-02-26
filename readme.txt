Web USB terminal emulator (well, without actual emulation :-)

This uses webusb/winusb or usbser to allow a webpage to become a terminal emulator for a cdc/acm serial port USB device!

You can filter USB devices by specifying vendorId and/or productId.

Click "USB" to connect to your cdc/acm serial port USB device thru webusb/winusb and communicate with its bulk endpoints
directly.

  * When using webusb/winusb your cdc/acm serial port USB device must not be claimed by usbser or you will get an access
    denied error.
  * You may need to edit the default endpoint numbers.

Or click "COMM" to connect to your cdc/acm serial port USB device thru usbser and communicate with its emulated comm port.

  * The Web Serial API needs to be enabled in your web browser thru:
    - edge://flags/#enable-experimental-web-platform-features
    - chrome://flags/#enable-experimental-web-platform-features
    - opera://flags/#enable-experimental-web-platform-features

Then enter commands in the command line!

Ctrl-C and Ctrl-D flow thru the command line when in focus.

Try it here: https://rtestardi.github.io/usbte/usbte.html
