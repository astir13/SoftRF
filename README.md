# SoftRF 
Multifunctional DIY IoT-based general aviation proximity awareness system, forked from http://github.com/lyusupov/SoftRF. This fork only supports the prime mkII hardware and provides some extra modifications to allow for following features:

# Features on top of SoftRF prime mkII
* external 12V powered (has a power supply)
* external equipment connected through 9-pin D-Sub connector
* power switch management that allows power control operation even if the SoftRF is hidden behind the instrument panel
* auto power off when on ground and no external power supplied
* supports NMEA devices like Flarm LED/LX devices through RS-232

# Documentation
* [User Manual](https://github.com/astir13/SoftRF/tree/master/documents/usermanual/binaries)
* Software
    * Firmware
        * [Binary Releases](https://github.com/astir13/SoftRF/wiki/Updates)
        * [Source](https://github.com/astir13/SoftRF/tree/master/software/firmware/source)
* Hardware
You need:
    * 1x TT-GO T-Beam v1.1 board with OLED display, like https://www.aliexpress.com/item/33050391850.html?spm=a2g0s.9042311.0.0.27424c4dU9WiWD
    * 1x RS-232/UART converter, like https://www.aliexpress.com/item/4000189810712.html?spm=a2g0s.9042311.0.0.27424c4dQ6D88f
    * 1x DC-DC 12V to 5V/3A converter as power supply, like https://www.aliexpress.com/item/32826540392.html?spm=a2g0s.9042311.0.0.27424c4dbbq0Ht
    * a chassis, 3D printed: https://www.thingiverse.com/thing:4704154/
    * some hot-glue
    * some wires
    * a protected Li-Ion battery, size 18650, 2600mAh or better, with integrated battery management system to give added security
    * a 9-pin sub-d female and male connector for soldering with matching srews to secure the corresponding counterpart with
    * a power ON-OFF-(ON) switch, like MS500D from Myiama Parts, e.g. https://www.reichelt.de/kippschalter-6a-125vac-1x-ein-aus-ein--ms-500d-p13156.html?CCOUNTRY=445&LANGUAGE=en&trstct=pos_0&nbc=1&&r=1
* Extras
    * see https://github.com/lyusupov/SoftRF

