# Clackotron 2000 - Hardware
This repository contains the hardware for the Clackotron 2000 project, which provides a simple, all-in-one solution for controlling SBB split-flap modules. For more information on the project in general, visit the [docs repository](https://github.com/clackotron/clackotron_docs).

The hardware is based around an ESP32-S3 and designed in KiCAD 7.0. The production files can be used to easily order the latest version of the PCB from a manufacturer. (JLCPCB)

Most notably, the hardware contains:
* 30V DC input and +/-/A/B connector (same as SBB split flap modules).
* Internal power supply for 5V (RS485) and 3.3V (ESP32-S3).
* An ESP32-S3 on which the [firmware](https://github.com/clackotron/clackotron_firmware) and [webinterface](https://github.com/clackotron/clackotron_webinterface) will run.
* A level converter for sending/receiving RS485 from the ESP32-S3.
* An RTC (PCF85263A) and battery for time-keeping while offline.
* Two buttons and a RGB-Led for misc. functionality.
