uDraw PS3 Linux Driver
======================

A driver for the PS3 uDraw graphics tablet modified by AkBKukU and originally by [Grumble](https://github.com/Grumbel/udraw). If customization is needed, hack the source. 

For a Windows driver, see: http://brandonw.net/udraw/


Requirements:
-------------
 - scons
 - libusb-1.0
 - boost
 - g++ 4.5 or above

Compilation:
------------

You will need to compile the source before you can run it. If you are running Ubuntu you can install the needed packages with `sudo apt-get install scons libusb-dev libboost-all-dev g++`. Then in the directory with the source files you can simply run `scons` to compile the source.


Running:
--------

Plug in the USB dongle for the graphics tablet, switch on the graphics
tablet and sync up as usual, then run `./udraw-driver` with one of the following flags to set the mode:

        --touchpad      use the device as touchpad
        --tablet        use the device as graphic tablet
        --gamepad       use the device as gamepad
        --keyboard      use the device as keyboard
        --accelerometer use the accelerometer
        --multi         use the device as graphic tablet and touchpad
        
If it doesn't launch you may need to run it as root.
