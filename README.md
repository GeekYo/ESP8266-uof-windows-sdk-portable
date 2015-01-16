# Espressif ESP8266 Windows SDK Portable Package

This is an attempt to convert the [Un-Official Windows SDK](http://www.esp8266.com/viewtopic.php?f=9&t=820)
into a workable and portable package that can be carried on a **USB stick!**

The assumption in mind is the system used has a **64-bit Architecture** with 
**Windows 7** or **Windows 8** as the operating system.

No additional Package needs to be installed, it works directly out of the box.

We have tried to bundle all the required utilities to make this most helpful for Windows Users.

## [Download ESP8266-UofWin-SDK-portable-v01.zip](https://drive.google.com/file/d/0B0LHhwkPhcG8VDlUN2Y3WUZuVTg/view?usp=sharing)

**MD5-SUM** = `3bd66a940d7ae913a9f4bf34991490e3`


## Additional Modules

1.  **Path Updater Utility** - *In case Examples are Imported into Eclipse* then one would need to 
    update the fixed path locations. This can be achieved by running the program
    `example-pathupdate\updatepath.exe` to make sure that all paths
    in the examples are updated. This utility also updates the **serial port** for 
    [*esptool*](https://github.com/themadinventor/esptool/) to load
    firmware. One just modify the *COM port* number in the file 
    `example-pathupdate\serial-port.txt` in a text editor 
    (only keep one line in the file).

2.  **Eclipse** version of *Luna 64-bit for Windows* is included with auto environment configuration
    using the `eclipse.cmd` file. By executing *this file* the Eclipse would automatically open 
    with the default workspace location `Workspace` Directory (in the present directory).

3.  **Direct Flasher** - This helps to program the single official Firmware image released from
    Espressif. This is located in the directory `ESP8266_directflasher`. This is the 
    [cloud update](https://docs.google.com/file/d/0B3dUKfqzZnlwVGc1YnFyUjgxelE/edit?pli=1)
    flasher that was released earlier. More details are available in the file 
    `ESP8266_directflasher\steps.txt`. It also contains the 
    [offical firmware](https://docs.google.com/file/d/0B3dUKfqzZnlwdUJUc2hkZDUyVjA/edit?pli=1)
    at this point of time in the file `ESP8266_directflasher\v0.9.2.2 AT Firmware.bin`.
    We have also packaged the famous **Node MCU's Lua Firmware** image in the file
    `ESP8266_directflasher\nodemcu_latest.bin`. For this direct flashing one 
    needs to power up the module in the * hardware configuration* mentioned in the
    `ESP8266_directflasher\steps.txt` file.

4.  **Cool Terminal** - We have included the famous [Roger Meier's Cool Terminal](http://freeware.the-meiers.org)
    in the `CoolTermWin` directory. This is an easy to use Serial port Terminal program to talk 
    and test out the ESP8266.

5.  **Node MCU's Flasher** in the Location 
    `ESP8266-nodemcu-flasher-master\ESP8266Flasher_x64.exe`
    to help in flashing of custom location using specific binary image files.
    Basically this an English version of the 
    [offical firmware loader](https://docs.google.com/file/d/0B3dUKfqzZnlwalVnM3lpMEdKRkk/edit?pli=1).

6.  **C++ Toolchain ** we have added the compiled *G++ xtensa toolchain for ESP8266* built by 
    [user igrr from esp8266 community forum](http://www.esp8266.com/viewtopic.php?f=9&t=820&start=80#p7349).
    However in order to use it one needs to modify the makefile to point at the correct path.
    This toolchain is located at `xtensa-lx106-elf-cpp\bin`. The original C toolchain
    is located at `xtensa-lx106-elf\bin` which came with the devkit package.


## Some Useful Images

### Bigger Picture of the ESP-01 Module:

![](https://raw.githubusercontent.com/boseji/ESP8266-uof-windows-sdk-portable/master/images/ESP8266-ESP01-boardpicture.jpg)


### ESP-01 module PCB layout View

![](https://raw.githubusercontent.com/boseji/ESP8266-uof-windows-sdk-portable/master/images/ESP-01 plate.png)


### Eclipse Path configuration for Code Complete in Windows SDK
![](https://raw.githubusercontent.com/boseji/ESP8266-uof-windows-sdk-portable/master/images/ESP8266-Windows-SDK-Codecompletion.png)


### ESP8266 Pin Configuration

![](https://raw.githubusercontent.com/boseji/ESP8266-uof-windows-sdk-portable/master/images/ESP8266EX Layout.jpg)


## License

This work has been released under GPLv2 by Boseji (c) 2015 
Unless otherwise explicitly specified in the individual parts of the package
all parts would be licensed under GPLv2. 
You can find this included as `LICENSE.txt` file.


## Foreword

Kindly let us know your feedback and issues for this package 

