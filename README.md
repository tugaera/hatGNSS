# hatGNSS
GSM/GPRS/GNSS HAT

SOURCE: https://www.waveshare.com/wiki/GSM/GPRS/GNSS_HAT

https://www.waveshare.com/wiki/File:CP210x_USB_TO_UART.zip

sudo raspi-config
Advanced Options -> Serial -> no, 
to disable Linux’s use of console UART Open /boot/config.txt file, find the below statement and uncomment it to enable the UART:

enable_uart=1

sudo apt-get install minicom

Execute command: minicom -D /dev/ttyS0（ttyS0 is the UART of Raspberry Pi 3B）

Baud rate is 115200 by default. If you need to change the baud rate, for example 9600, you can add the parameter -b 9600.

The user UART device of Raspberry Pi 2B/Zero is ttyAMA0, and ttyS0 of Raspberry Pi 3B 
