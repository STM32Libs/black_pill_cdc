# STM32F411CE Black Pill USB example
in STM32CubeMX
* RCC HSE Crystal
* Connectivity : USB_OTG_FS, Mode Device_Only
* Middleware : Class For FS IP, Virtual Port Com
* GPIO PC13 as output for LED

## Fixing ST-Link debug problem
* Edit configuration / Debugger / Show generator options => Software System Reset

## Fixing USB port error
* Error : Unable to open connection to COMX Unable to configure serial port
* Fix applied in this repo in `USB_DEVICE\App\usbd_cdc_if.c` : https://community.st.com/s/question/0D50X00009Xke3ESAR/usb-vcp-windows-10

# References
* [STM32-base Black Pill V1.2](https://stm32-base.org/boards/STM32F401CCU6-WeAct-Black-Pill-V1.2)
* [USB-C Black pill schematics](https://stm32-base.org/assets/pdf/boards/original-schematic-STM32F411CEU6_WeAct_Black_Pill_V2.0.pdf)
* [Reference Manual](https://www.st.com/resource/en/reference_manual/dm00119316-stm32f411xce-advanced-armbased-32bit-mcus-stmicroelectronics.pdf)
