# Flash-Multi
Tool for flashing pre-compiled firmware to an STM32-based Multiprotocol TX module via an FTDI adapter or the built-in USB connection. 

<p align="center">
  <img src="img/flash-multi.jpg">
</p>

# Supported Modules
* Jumper JP4IN1
* iRangeX IRX4, IRX4 Plus, and IRX4 Lite
* Vantac MPM Lite
* 'Banggood' STM32 Multiprotocol TX Modules
* DIY STM32 Multiprotocol TX Modules

# Installation
1. Download the .zip archive of the latest version from the Releases page
1. Unzip the archive to a convenient location

# Usage
**Note for IRX4, Banggood, and DIY modules:** The first time you flash your module you will need to connect it with an FTDI adapter in order to flash the bootloader. The bootloader is required in order for the USB port to work and it can only be written with an FTDI adapter.

**Note for FTDI connections:** When using an FTDI adapter the `BOOT0` pin on the board must be connected to 5V, usually by installing a jumper on the `BOOT0` header pins.

1. Connect your module using the USB port or via an FTDI adapter, as appropriate.  Note the COM port which appears when the device is connected.
1. Double-click `flash-multi.exe`
1. Click the **Browse** button and locate a compiled firmware file
1. Select the appropriate COM port
1. Click the **Go** button

# More Information
Much more information about flashing a Multiprotocol module, including how to [compile from source](https://github.com/pascallanger/DIY-Multiprotocol-TX-Module/blob/master/docs/Compiling_STM32.md) and how to connect an FTDI adapter and connect the `BOOT0` pin, can be found in the documentation for the DIY Multiprotocol Module at https://github.com/pascallanger/DIY-Multiprotocol-TX-Module.