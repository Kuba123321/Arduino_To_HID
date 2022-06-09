!You do it at your own risk!

# Arduino_To_HID
Turn arduino to HID device
After that your arduino will be deteced as HID(keyboard), beacouse of that you will be able to run your code.

First you need to download - Atmel Flip, Arduino IDE, arduino-keyboard.hex - https://github.com/coopermaa/USBKeyboard/blob/master/firmware/Arduino-keyboard-0.3.hex, Arduino-usbserial-atmega16u2-Uno-Rev3.hex - https://github.com/arduino/ArduinoCore-avr/blob/master/firmwares/atmegaxxu2/arduino-usbserial/Arduino-usbserial-atmega16u2-Uno-Rev3.hex to restore arduino to normal COM
Go to Arduino IDE create new project.
Add HID Libary   https://github.com/SFE-Chris/UNO-HIDKeyboard-Library
On this repository you can find some examples and understand how the code work

After you write you code click on upload on left top corner (important in IDE you have to chose COM3 under tools-port-COM3)
Next you have to put ARDUINO in DFU mode to do that you need to short ![image](https://user-images.githubusercontent.com/90273406/170819092-6b1f80ac-9716-4226-bfa9-1fed6730d968.png)

Next go to the Atmel Flip
Click on Device Selection and select yours microprocesor for my arduino uno r3 is ATmega16u2 click OK. Then click on next icon (USB) select USB or press ctrl-u.
On top menu select File-Load Hex file-Find arduino-keyboard.hex localisation and select it. After that click run. To see efects you need to unplug arduino and plugi in again. 

================================================================================================================================================================
How to get arduino back in COM mode.



When you plug your arduino you need to short the pins again. Then go to the Atmel Flip as same as before, you need to select Arduino-usbserial-atmega16u2-Uno-Rev3.hex then upload it. Unplug arduino and plug it again.


