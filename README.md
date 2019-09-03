# RPi_Teensy_HexLoader
WIP to attempt a simple HEX loader from Raspberry Pi.

## Specs
We'd like to be able to have a simple, easy to use HEX loader usable at our manufacturing facility, or at end user sites for updating code. Some basic goal specs:
  - simple to use with no instructions
  - low cost so if lost or destroyed no big tears
  - small touchscreen HAT for simple GUI
    - loads default file only, no selection needed. File could be located on RPi or the SD card so easily updated.
    - shows successful connection to Teensy and it's VID and PID, or 'No Teensy' if not
    - shows the name of the file found in the default load folder
    - shows success or not
    - keeps running count of number of good and bad loads
  - some simple way to keep people from stealing the HEX file? Would not do them much good anyway.
  - Raspberry Pi 3 or 4
  - loads premade HEX file via Teensy USB. We mainly use T3.2 but should work with any Teensy.
  - USB power supply with wall wart

## References and resources
  1. PJRC [Linux loader C code](https://www.pjrc.com/teensy/beta/load_linux_only.c)
  2. PRJC support forum [thread about firmware loaders](https://forum.pjrc.com/threads/799-Firmware-loader-for-Teensy-3) with many links to code and examples there.
  3. Windows-only C# project: [C# Windows helper classes for Teensy comms at GitHub](https://github.com/luni64/TeensySharp) with a recently-added sample app. Still, the code might be helpful on Linux.
  4. Teensy loader, command line [page at PJRC](https://www.pjrc.com/teensy/loader_cli.html) with many links
  5. teensy_loader_cli [repository at GitHub](https://github.com/PaulStoffregen/teensy_loader_cli) also linked from (4)
