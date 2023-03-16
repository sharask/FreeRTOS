# FreeRTOS USB demo project<br>

STM32F407-Disc1 kit<br>
STM32CubeIDE 1.11.2<br>

CDC Class (Virtual COM port) used to send data from MCU through USB.<br>
Problem: if we try to send two messages without delay between them, second message won't be sent due bussy USB peripheral.<br>

It this project two tasks write messages to freertos queue.<br>
Dedicated task *StartUSBPrintTask()* takes these messages from queue and outputs over USB.<br>
After the message is successfully transmitted through the USB, callback function *CDC_TransmitCplt_FS()* is fired.
In this callback function we can use "Direct task notification" to inform about empty USB buffer and give permission to send next message.


