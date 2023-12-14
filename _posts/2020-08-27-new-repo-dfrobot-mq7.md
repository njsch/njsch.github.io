---
title:  "New Working Project Repository -- DFRobot_MQ7_CO_data_logging"
date:   2020-08-27 22:50:00 +1100
categories: CompSci GitHub Technology Hardware Firmware Arduino UNO UNOr3 Microcontroller DFRobot.
description: "A new code repository has been added to my GitHub account: DFRobot_MQ7_CO_data_logging.  To be strictly accurate, I didn't..."
---

A new code repository has been added to my GitHub account: [DFRobot_MQ7_CO_data_logging](https://github.com/njsch/DFRobot_MQ7_CO_data_logging/).  To be strictly accurate, I didn't write much of it: it is a collation of several different appropriately credited coding sources.

It allows for data to be collected from a basic hardware Carbon Monoxide sensor, namely the [DFRobot](https://www.dfrobot.com/) [MQ7](https://core-electronics.com.au/analog-carbon-monoxide-sensor-mq7.html).  It collects gas readings between 20 and 20,000 [particles per million (PPM)](https://groups.molbiosci.northwestern.edu/holmgren/Glossary/Definitions/Def-P/parts_per_million.html).  when collecting the data, it logs the results to a [Comma-separated values (CSV)](https://www.csvreader.com/csv_format.php) file on an inserted SDHC memory card.

It has been tested and runs well on an [Arduino UNO](https://www.arduino.cc/en/Guide/ArduinoUno) [r3](https://store.arduino.cc/usa/arduino-uno-rev3) with an [Arduino-compatible data logging shield](https://www.jaycar.com.au/arduino-compatible-data-logging-shield/p/XC4536).  The sensor requires at least four pins (including the data logging) for this code to work (one analog, one digital, one 5v and one ground).

Obviously, it requires external calibration for the data to be accurate, which can only be done if you have another sensor to compare with, or use a calibration kit.  Licensed under GNU LGPL as necessitated by DFRobot.

## Usage:
It is relatively simple to use and implement.  If you purchase an arduino board, all you have to do is just:
* [download](https://www.arduino.cc/en/main/software) the Arduino integrated development environment (IDE) for free.
* Clone or release-download the code.
* Import it into the Arduino IDE as a new sketch.
* Use either the [Arduino IDE Library Manager](https://www.arduino.cc/en/guide/libraries) or manually install the following two libraries:
  * The [Adafruit](https://www.adafruit.com/) [Common Sensor Library](https://github.com/adafruit/Adafruit_Sensor); and
  * The Adafruit [Real-time Clock Library (RTCLib)](https://github.com/adafruit/RTClib).
* Connect the Arduino board over USB and make sure that it is registered / assigned to the right COM ports in IDE > tools menu > COM Ports - possibly turn bluetooth off as well.
* Press Control+R to verify and compile the code.
* Finally press Control+U to transfer / upload the compiled program to the board.  Should start working after that - check the upload out and serial moniter.

If you are allergic to graphical interfaces, or are sight-impaired and / or do not have the [Java Access Bridge (JAB)](https://docs.oracle.com/javase/accessbridge/2.0.2/introduction.htm) &ndash; which is quite out-of-date anyway and will probably become increasingly unusable over the years &ndash; then you can always use the [Arduino-CLI](https://www.arduino.cc/pro/cli), the Arduino command-line interface (CLI).  This simplifies the process even more, if you are used to text-based computer interaction.  Also, NVDA is the only screen-reader that reliably works with the IDE, whereas JAWS crashes nearly every single time for some reason.

I was originally thinking of using this code for an assignment; however, this is no longer viable for certain ethical reasons.  So the code is now publicly available.