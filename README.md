# STM32L10X_MSD_BOOTLOADER
Mass Storage Device Bootloader for STM32L1XX

Tested with STM32L100R8T6.

Basicklly, only the BTN is needed.


Usage
1. Keep BTN pressing before plugin the usb cable, until the LED blinks;
2. Drag and drop the bin file into the simulate flash drive;
3. If you don't have app in the flash yet, it will enter the MSD mode no mater the BTN is pressed or not;
4. In MSD mode, press and hold the BTN for about 2S, the LED will keep lighting then release it, device will restart.;


Bootloader size define:

![](https://github.com/lingex/STM32L10X_MSD_BOOTLOADER/blob/master/bl%20size.png)

PINOUT:
![](https://github.com/lingex/STM32L10X_MSD_BOOTLOADER/blob/master/PINOUT.png)

The PWR_EN USB_EN BTN_GND pin is not necessary, depends your board.
No need to care about the flash size, erase page size.



Thanks to:
https://github.com/sfyip/STM32F103_MSD_BOOTLOADER.git
https://community.st.com/s/question/0D50X00009ho3Fy/procedures-for-developing-an-stm32-bootloader-app
