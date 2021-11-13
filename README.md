#GL_C/Embedded_BaseCamp

This is repo for my future projects in BaseCamp

additional info could be found on [GoogleDrive](https://drive.google.com/drive/folders/1tlN19uFuyV8WtB7ZqKWShtZ0hcubU_r1?usp=sharing)

Wokshop_1:
implement custom blinking sequence with 4 leds

Workshop_2:
implement at least 3 blinking schemes for all 4 LEDs on the board
2 buttons would be used to select scheme (next one, previous one).
2 buttons would be used to select blinking speed (speed up, slow down).
Button at the middle of cross should be used to turn on/off blinking.
All buttons need to be processed by interrupts.

Workshop_3:
implement PWM signal generator.
Time4 need to be used (this is mandatory).
STM32F407 need to be switched for external clock (HSE).
2 buttons would be used to set signal frequency (up and down; +/- 5 kHz step).
2 buttons would be used to set duty cycle (+/- 5% step each button press).
Middle button would be used to select signal output (PD15, PD14, PD13, PD12 or no output (disable case)). Cyclic selection scheme.

Workshop_4:
Need to read voltage from potentiometer (connect it to IN3 channel). Show voltage with help of BLUE led (light intensity change). Too high voltage needs to be indicated with RED led (see p.4).
Need to read temperature from internal temperature sensor (inside STM32F407). Show temperature with help of ORANGE led (light intensity change). Too high temperature needs to be indicated with RED led (see p.4).
Need to read temperature from external analog temperature sensor (present at GL board). Show temperature with help of GREEN led (light intensity change). Too high temperature needs to be indicated with RED led (see p.4).
RED led should be turned off if no “emergency citation” present (see p.1,2,3 “too high cases”). It should bling with 1Hz frequency if we have “one emergency situation”, it should blink with 2.5Hz frequency for case when we have 2 “emergency situations” at the same time. And 5Hz – if all 3 “emergencies” present.

Workshop_5: 
Need to start UART3 with following settings: baud rate 115200, 8bit, no parity, 1 stop bit.
Need to control all 4 LED states with help of the PC keyboard. Keyboard button toggles LED state (via console). 
Need to control all 4 LED states with help of buttons SWT1, SWT3, SWT4, SWT5 (on the GL board) – toggle mode.
One time per 5 seconds, actual temperature (external analog sensor at GL board) value should be printed at console (Celsius degrees).
[*OPTIONAL]. Create SW at PC to handle functionality that listed above (p. 2, 4) instead of console.
