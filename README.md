# DefineOS-andriod
An Andriod ROM custom-built to be as minimalist and fast as possible.

# Supported Devices [as of now]
Tecno Spark 20c

# Upcoming Devices
Infinix Smart 7

# Required Tools
A Windows Device
, ADB
, Shizuku 
, DSU Sideloader
, Your device's stock rom vbeta.img file [optional]


# How to install? [Do it at your own risk, we are not responsible for the damanges, or a bricked device, or world war 3]
go to adb shell then do:
adb reboot bootloader |
wait for you device to reboot and then:
fastboot erase system_a
|make sure our system.img from the releases in in the same folder as your adb files and then do: fastboot flash system_a system.img | and then: fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img[your stock rom's vbeta img] {this is optional, only needed if the device bootloops}
| and finally do: fastboot -w
| after these reboot your system and if it tells you that your data is corrupted and need to factory reset then do it and it will boot into DefineOS 



