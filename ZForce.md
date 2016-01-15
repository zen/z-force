# Z-Force #

## Z-Wave packet interception and injection tool ##

  * Authors: Behrang Fouladi, Sahand Ghanoun
  * Source Code: To be released mid-September 2013 on [Google Code](https://code.google.com/p/z-force)
  * Hardware Requirements: [CC1110 RF Transceiver](http://www.ti.com/tool/cc1110dk-mini-868), USB to UART Bridge
  * Release Date: 14/08/2013

Z-Force is a radio modem that can intercept and inject raw Z-Wave frames including encrypted packets to arbitrary destinations and Z-Wave Home IDs. It was developed during our research project on Z-Wave home automation systems which was presented in BlackHat 2013 USA conference. Z-Force toolkit consists of the following hardware and software components:

  * Two CC1110 RF transceivers used as receiver and transmitter interfaces
  * CC1110 chip Firmware that loosely implements Z-Wave physical and transport layers
  * Two USB to UART bridge to facilitate communication with RF boards over virtual COM ports
  * A GUI program written in C# that displays the intercepted Z-Wave frames and their payloads as well as enabling the user to replay a captured packet or send raw packets with arbitrary fields and payloads.

Setting up Z-Force hardware is straightforward: upload the RX and TX firmwares to receiver and transmitter CC1110 boards using Texas Instruments [SmartRF Flash Programmer](http://www.ti.com/tool/flash-programmer) and connect them to your PC or laptop via USB to UART bridge. The following pictures show the required USB-UART bridge connections to CC1110 I/O connector pins:

<p align='center'><img src='http://drive.google.com/uc?export=view&id=0B8l07E7STihRM3VyRmx2YTdrMFU&nonsesnse=something.png' /><br><i>Connections to CC1110 I/O pins</i><br><font color='red'><b><i>Please note External Power in the above picture is +3.3V and not +5V!</font></i>

After configuring the virtual COM port numbers associated with the receiver and transmitter boards in the GUI program, the kit is ready to intercept and send Z-Wave packets.</b>

<p align='center'><img src='http://drive.google.com/uc?export=view&id=0B8l07E7STihRMDc4TlJBSXZ6NjA&nonsesnse=something.png' /><br><i>Z-Force GUI</i>