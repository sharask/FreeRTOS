# FreeRTOS Tasks demo project

STM32F407-Disc1 kit<br>
STM32CubeIDE 1.12.0<br>

Three tasks created: DefaultTask, SendingTask, ReceivingTask<br>
- SendingTask sends command from user-defined type *LED_COMMANDS* through the Queue<br>
- ReceivingTask waits for the command and switches on/off Leds according received command<br>
- Debug messages are send to the ITM data console<br>
