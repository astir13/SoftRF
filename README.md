# SoftRF &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [![Join the chat at https://gitter.im/lyusupov/SoftRF](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/lyusupov/SoftRF?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](https://travis-ci.org/lyusupov/SoftRF.png?branch=master)](https://travis-ci.org/lyusupov/SoftRF "Build Status") 
Multifunctional DIY IoT-based general aviation proximity awareness system.

Features:
* 2-way raw data bridge between 868/915 MHz radio band and Wi-Fi ;
* standalone, battery powered, compatible proximity awareness instrument that fits typical 2.25 inches hole ;
* lightweight version to carry onboard of an UAV.

# Compatibility <sup>1</sup>
Type|Protocol|FLARM|OGN tracker|PilotAware|Skytraxx|SoftRF
---|---|---|---|---|---|---
Radio|FLARM AIR V6|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>|||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_yellow_32.png)<sup>2</sup></p>|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>
&nbsp;|<p align="center">OGNTP</p>||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>|||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)<sup>3</sup></p>
&nbsp;|<p align="center">P3I</p>|||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)<sup>3</sup></p>
&nbsp;|<p align="center">UAT&nbsp;978</p>|||||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)<sup>4</sup></p>
&nbsp;|<p align="center">FANET+</p>||||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)<sup>3</sup></p>
Data|FLARM NMEA|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>
&nbsp;|Garmin GDL90|||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>
&nbsp;|<p align="center">MAVLINK</p>|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>|<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>|||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>
&nbsp;|<p align="center">Dump1090 &nbsp;<sup>5</sup></p>|||||<p align="center">![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/check-mark_32.png)</p>

<sup>1</sup> - it is necessary for a reader to distinguish the difference between statement "**compatible**" and statement "**fully compatible**".<br>
&nbsp;&nbsp;&nbsp;&nbsp; SoftRF implements only a reasonable minimum of the protocols specs. No "bells and whistles" so far.<br>
<sup>2</sup> - FANET+ can not receive FLARM. However it is able to transmit it.<br>
<sup>3</sup> - valid for [**Prime Mark II**](https://github.com/lyusupov/SoftRF/wiki/Prime-Edition-MkII) and [**Dongle**](https://github.com/lyusupov/SoftRF/wiki/Dongle-Edition) **Editions**; valid for **Standalone** and **UAV** **Editions** with optional DIY [SoftRF LoRa RF module](https://github.com/lyusupov/SoftRF/wiki/SoftRF-LoRa-module)<br>
<sup>4</sup> - [**Reception**](https://github.com/lyusupov/SoftRF/tree/master/software/firmware/source/UATbridge) of traffic 'downlink' frames only. Valid for **Standalone Edition** with optional DIY [SoftRF UAT module](https://github.com/lyusupov/UAT-test-signal#variant-2-advanced)<br>
<sup>5</sup> - also known as "raw ADS-B"<br>

# Models
Model|Platform|First appearance|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Status&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|Comment
---|:---:|:---:|:---:|---
1&nbsp;[Prime](https://github.com/lyusupov/SoftRF/wiki/Prime-Edition)<br>2&nbsp;[Standalone](https://github.com/lyusupov/SoftRF/wiki/Standalone-Edition)<br>3&nbsp;[UAV](https://github.com/lyusupov/SoftRF/wiki/UAV-Edition)|[Espressif<br>ESP8266](https://en.wikipedia.org/wiki/ESP8266)|Q4 2015|![](https://placehold.it/140x70/00A000/000000?text=Good)|[Prime](https://github.com/lyusupov/SoftRF/wiki/Prime-Edition) model is no longer supported - use [Prime MkII](https://github.com/lyusupov/SoftRF/wiki/Prime-Edition-MkII) instead.<br>ESP8266 platform will be phased out through year 2020 in favour of ESP32.
1&nbsp;[**Prime Mark II**](https://github.com/lyusupov/SoftRF/wiki/Prime-Edition-MkII)<br>2&nbsp;[**Standalone**](https://github.com/lyusupov/SoftRF/wiki/Standalone-Edition) + [adapter](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER)<br>3&nbsp;[UAV](https://github.com/lyusupov/SoftRF/wiki/UAV-Edition)<br>4&nbsp;[**SkyView EZ**](https://github.com/lyusupov/SoftRF/wiki/SkyView-EZ)<br>5&nbsp;[Flight Recorder](https://github.com/lyusupov/SoftRF/wiki/Flight-Recorder)|[Espressif<br>ESP32](https://en.wikipedia.org/wiki/ESP32)|Q1 2018|![](https://placehold.it/140x70/00A000/000000?text=Good)|Today's best platform
1&nbsp;[**Raspberry Edition**](https://github.com/lyusupov/SoftRF/wiki/Raspberry-Edition)<br>2&nbsp;SkyView Pi|[Broadcom<br>BCM283X<br>(Raspberry Pi)](https://en.wikipedia.org/wiki/Raspberry_Pi)|Q4 2018|![](https://placehold.it/140x70/00A000/000000?text=Good)|Good for use together with RTL-SDR dongles to achieve additional 1090ES (and 978UAT) ADS-B air traffic reception.
[UAT module](https://github.com/lyusupov/UAT-test-signal#variant-2-advanced)|[Texas Instruments<br>CC13XX](http://www.ti.com/product/cc1310)|Q1 2019|![](https://placehold.it/140x40/c5f015/000000?text=May+need)<br>![](https://placehold.it/140x40/c5f015/000000?text=improvements)<!-- ![](https://placehold.it/140x70/FFFF00/000000?text=In+progress)-->|Resources of this platform are not sufficient to fit full SoftRF firmware.<br>Unique RF radio specs are useful for [UAT reception](https://github.com/lyusupov/SoftRF/tree/master/software/firmware/source/UATbridge) [ [1](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/uat-normal-7.jpg) , [2](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/uat-normal-8.jpg) , [3](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/uat-normal-6.jpg) ].
1&nbsp;[**Dongle**](https://github.com/lyusupov/SoftRF/wiki/Dongle-Edition)<br>2&nbsp;[Retro](https://github.com/lyusupov/SoftRF/wiki/Retro-Edition)|[STMicroelectronics<br>STM32](https://en.wikipedia.org/wiki/STM32)|Q3 2019|![](https://placehold.it/140x70/00A000/000000?text=Good)<!-- ![](https://placehold.it/140x70/FFFF00/000000?text=In+progress)-->|[AcSiP **S76G**](http://www.acsip.com.tw/index.php?action=products-detail&fid1=19&fid2=&fid3=&id=41&lang=3) "3-in-1" system-in-package **is doing good** [ [1](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/watch-1.jpg) , [2](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/t-motion-4.jpg) , [3](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/t-motion-5.jpg) ] .<br>As well as STM32F103C8 "**Blue Pill**" (same MCU that [STM32 OGN tracker](http://wiki.glidernet.org/stm32-ogn-tracker) uses) [ [4](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/stm32_breadboard.jpg) , [5](https://raw.githubusercontent.com/lyusupov/SoftRF/master/documents/images/stm32_ognweb_1.JPG) ] .

# Documentation
* [User Manual](https://github.com/astir13/SoftRF/tree/master/documentation/usermanual/binary/)
* Software
    * Firmware
        * [Binary Releases](https://github.com/astir13/SoftRF/wiki/releases)
        * [Source](https://github.com/astir13/SoftRF/tree/master/software/firmware/source)
* Extras
    * see https://github.com/lyusupov/SoftRF

