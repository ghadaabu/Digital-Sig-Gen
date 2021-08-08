# Digital-Sig-Gen

This project works with MSP430 using Assembly, it generates a Digital signal by converting a binary number into a continuous signal.  
First, a menu shows up on the LCD as follows:
1. Instructions 
2. Modulation Frequency 
3. Sync Frequency 
4. Action 
5. Quit

By clicking the desired number from the Key-Pad, options can be chosen, while rolling up and down is made with the Push-Buttons as follows: 
* PB1: Left 
* PB2: Up 
* PB3: Down
* PB4: Right  
-------------------------------------  
Explanation for menu options:  
1. Instructions: Prints Project's name and the number of Pin that should be connected to the Scope.
2. Modultion Frequency: Prints optional modulation frequency values. ( 2Khz 4KHz 6KHz )
3. Sync Frequency: Prints optional syncronic frequency values. ( 1Khz 2KHz )
4. Action: Generates a digital signal which follows the required frequences, using DAC0 while the signal cosists of two parts, the syncronic part, a continuos rectangular signal with the choosen frequency and the modulation part, which is modulation of a binary number choosen with the Key-Pad. (triangle signal for the bit 1 and zero sinal for the bit 0)
5. Quit: Stops the program and goes sleep mode.
