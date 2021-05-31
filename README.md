# Serial-Bootloader-STM32F407
change your application parameters as below:  -> In the system_stm***.c change VECT_TAB_OFFSET from 0x00000000U to 0x00008000U.  -> In both STM32F407VGTX_FLASH.ld and STM32F407VGTX_RAM.ld files change line as follow:  
FLASH    (rx) : ORIGIN = 0x8008000,   LENGTH = 992K
USE SERIAL PORT3

-> flash MCU with bootloader.bin file
-> use software to flash Application.bin file
-> connect your board to PC via serial port 3. then press Connect button and re-plug board power. if Connection successful press Program button to flash your MCU! 

![img](https://github.com/MahmoodShabanifard/Serial-Bootloader-STM32F407/blob/main/Screenshot%202021-05-31%20230027.png)
