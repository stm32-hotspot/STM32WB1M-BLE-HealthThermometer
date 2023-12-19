# BLE Health Thermometer 

## Application Description

This ***BLE_HealthThermometer*** application uses the temperature sensor embedded on the **B-WB1M-WPAN1 board** to transmit and display the temperature data on an **Android or IOS device**. 

For more information regarding the B-WB1M-WPAN1 board, please visit: 
https://www.st.com/en/evaluation-tools/b-wb1m-wpan1.html


## Hardware and Software environment

  - This application runs on B-WB1M-WPAN1 board
  - B-WB1M-WPAN1 board Set-up
    - To power the board use USB cable type A to USB type C connector through MB1880 board or use CN4 connector (Pin 1 : GND, Pin 2 : 5V)
    - Use an external STLINK-V3 in order to flash the binary

## How to use it ? 

This application requires having the stm32wb1x_BLE_Stack_full_fw.bin binary flashed on the Wireless Coprocessor.
If it is not the case, you need to use STM32CubeProgrammer to load the appropriate binary.
All available binaries are located under /Projects/STM32_Copro_Wireless_Binaries directory.
Refer to /Projects/STM32_Copro_Wireless_Binaries/ReleaseNote.html for the detailed procedure to change the
Wireless Coprocessor binary or see following wiki for Hardware setup:
https://wiki.st.com/stm32mcu/wiki/Connectivity:STM32WB_BLE_Hardware_Setup

In order to make the program work, you must do the following:
 - Open your toolchain 
 - Rebuild all files and flash the board with the executable file

 On the Android/IOS device, enable the Bluetooth communications, and if not done before,
 - Install the ST BLE Sensor and/or ST BLE Toolbox applications:
    https://wiki.st.com/stm32mcu/wiki/Connectivity:BLE_smartphone_applications#ST_BLE_Toolbox

 - Power on the B-WB1M-WPAN1 board with the BLE_HealthThermometer application
 - Then, click on the App icon, STM32 BLE Toolbox (android device)
 - select the HTSTM in the device list
 - connect the application
 - open Health Thermometer service

The temperature is displayed each second on the Android/IOS device.

Available Wiki pages:
  - https://wiki.st.com/stm32mcu/wiki/Connectivity:BLE_overview

For more details refer to the Application Note:
  AN5289 - Building a Wireless application
 
## Troubleshooting

**Caution** : Issues and the pull-requests are **not supported** to submit problems or suggestions related to the software delivered in this repository. The STM32WB BLE_HealthThermometer example is being delivered as-is, and not necessarily supported by ST.

**For any other question** related to the product, the hardware performance or characteristics, the tools, the environment, you can submit it to the **ST Community** on the STM32 MCUs related [page](https://community.st.com/s/topic/0TO0X000000BSqSWAW/stm32-mcus).