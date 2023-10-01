# Analog Discovery RS-232 five wire sniffer add on circuit
## Motivation
While troubleshooting an old but extremely robust threadmill, I came across an RS-232 data link between the device and its master computer. Since I do not have any instruments to sniff the messages flowing through a RS-232 link, I decided to build an extension board to add this capability to my Analog Discovery II instrument (AD). To give myself more flexibility, I am adding plenty of headers to monitor extra signal lines in addition to the main RxD and TxD. A total of five lines can be monitored at any time.

## Warnings
Use it at your own risk. I take no responsibility for any damage caused to any device attached to this board. Since this is an experimental circuit, I assume that whoever is reading this is a tinker and has basic skills dealing with extra-low-voltage circuits.

## Features
* Uses the [Texas Instrument TRSF3243EIPWR Multichannel RS-232 compatible line driver/receiver](https://www.ti.com/product/TRSF3243E)
* Five channel rs232 sniffer
* RxD and TxD lines always connected to AD instrument DIO0-1
* Selectable signals can be connected to the AD DIO2-4 via header shunt pins
* RxD and TxD signals connected to AD instrument oscilloscope channels
* Optionally, RxD and TxD can be driven by an AD instrument using DIO7-8
* It is also possible to select one more signal line to be driven by an AD instrument DIO9
* The driver power can be enable(disable) driving the DI15 high(low)




## Required equipment:
* A data link with RS-232 communication to sniff on
* Personal Computer
* Digilent Analog Discovery (R) Instrument
* Software Digilent Waveforms(R)
* Some extra db9 terminated cables to make the connections

## License

Analog Discovery (R) and Waveforms(R) are Digilent trademarks.
The license is described in the file 'LICENSE'.
