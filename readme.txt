USBTE -- Web USB Terminal Emulator (well, without actual emulation :-)

This uses webusb/winusb or usbser to allow a webpage to become a terminal emulator for a cdc/acm serial port USB
device!

You can filter USB devices by specifying VID and/or PID.

Click "COM" to connect to your cdc/acm serial port USB device thru usbser and communicate with its emulated comm
port.

  * The Web Serial API needs to be enabled in your web browser thru:
    - edge://flags/#enable-experimental-web-platform-features
    - chrome://flags/#enable-experimental-web-platform-features
    - opera://flags/#enable-experimental-web-platform-features

Or click "USB" to connect to your cdc/acm serial port USB device thru webusb/winusb and communicate with its bulk
endpoints directly.

  * On Windows, your USB device must not be claimed by usbser.sys or you will get an access denied error.
  * On Windows, you must manually update "Universal Serial Bus devices" -> "WinUsb Device" driver to your device.
  * You may need to edit the default endpoint numbers.

Then enter commands in the command line!

Ctrl-C and Ctrl-D flow thru the command line when in focus.

Try the USB Terminal Emulator here: https://rtestardi.github.io/usbte/usbte.html
