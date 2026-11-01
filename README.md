# TurboLoad Sock & Load Edition

![TurboLoad Sock & Load Edition](images/1.jpg)
![TurboLoad Sock & Load Edition](images/2.png)
![TurboLoad Sock & Load Edition](images/3.jpg)

## Description
A clone of the Australian designed C64 HES/HPD Turboload Cartridge for C64 Disk Drives

**Features**
* Speeds up the load of floppy disks by up to 6 times
* Adds additional DOS commands
* Create and load disk menus
* Reset Button
* Power LED
* Compatible with the JACC64 case

## Bill of Materials

| Qty | Component                    |
|:---:|------------------------------|
| 1   | 470nF Tantalum Capacitor     |
| 2   | 100nF Ceramic Capacitors     |
| 1   | 5mm LED                      |
| 1   | 330Ω Axial Resistor (LED)    |
| 1   | 4.7KΩ Axial Resistor         |
| 1   | 10KΩ Axial Resistor          |
| 1   | 6mm Tactile Switch           |
| 1   | 74LS09 14pin DIP             |
| 1   | 27C64 or compatible (E)EPROM |

* IC sockets optional.
* The LED resistor is nominally 330Ω but anything up to 1K usually is fine
* Larger EPROMS/EEPROMS can generally be used but repeat the image to fill up the ROM

## DOS Commands
Typing @H and RETURN will bring up a help screen which lists the commands.

### @
Toggle TURBOLOAD on and off. The screen colours will be C64 standard when TURBOLOAD is off, but will change when TURBOLOAD is on. Other features remain available when TURBOLOAD is off.

### @$
Display the disk directory. This will remove current programs in memory. The listing may be paused by pressing any key. Pressing any key again will resume listing. Pressing the RUN/STOP key will return the READY prompt.

### @B
List a BASIC program in memory to a Commodore compatible printer (device number 4).

### @E
Reads the error channel to display the error type and stop the disk drive error light flashing.

### @D"Filename"
Deletes the file. Files may be deleted using the directory listing by typing @D on the left of the screen, making sure that there are only blank spaces between the @D and the quote mark at the left of the program name.

### @F"Diskname,ID"
Complete format (for new disks).

### @F"Diskname"
Short format, clears the disk directory (existing programs may be recoverable – refer to disk drive manual).

### @L"Filename"
Loads a program, equivalent to LOAD"Filename",8,1. Files can be loaded using the directory listing by typing @L on the left of the screen, making sure that there are only blank spaces between the @L and the quote mark at the left of the program name.

### @L
Loads the first file on the disk.

### @M
Displays the TURBOMENU screen (refer next section).

### @P
Dumps screen text to a Commodore compatible printer (device number 4). This can also be called from within a program by using SYS57046.

### @V
Validates a disk.

### @"Command"
Sends a command to the disk drive (e.g. @"R0:new name=old name" to rename a file).

## 3D Printable Case
This PCB is designed to be compatible with the case for the JACC64-16K cartridge. Please see that repository for details.

## Support Me
Everything is freely available so you can make your own PCB and case, however if you would like to support me, please see the following links.

* [My Projects](https://projects.amiga-hardware.com) - Donate on this page
* [Order the TurboLoad Sock & Load PCB]()
* [Order the JACC64-16K Case which is compatible](https://www.pcbway.com/project/shareproject/JACC64_16K_C64_Cartridge_Case_78ec0fd1.html)

