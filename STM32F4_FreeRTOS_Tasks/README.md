# FreeRTOS Tasks demo project

STM32F407-Disc1 kit<br>
STM32CubeIDE 1.12.0<br>

Three tasks created: DefaultTask, GreenTask, BlueTask<br>
GreenTask and BlueTask toggle Leds and send messages to the ITM data console<br>

Additionaly, to get valid RTOS run-time statistics RUN-TIME-STATS enabled and macros in the freeRTOSConfig.h file defined.<br>
- To se statistics, open menu *Window->Show View->FreeRTOS->FreeRTOS Task List*<br>
