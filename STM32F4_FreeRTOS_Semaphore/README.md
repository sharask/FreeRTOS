# FreeRTOS Semaphore demo project

STM32F407-Disc1 kit<br>
STM32CubeIDE 1.12.0<br>

Three tasks created: DefaultTask, GreenTask, BlueTask<br>
- GreenTask sends Semaphore signal.<br>
- BlueTask waits for the Semaphore signal. After receiving signal blinks blue led 3 times.<br>
- Debug messages are send to the ITM data console.<br>
