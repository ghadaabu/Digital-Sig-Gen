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
### Menu options 
1. Instructions: Prints the Project's name and the number of pins that should be connected to the Scope.
2. Modulation Frequency: Prints optional modulation frequency values. ( 2Khz 4KHz 6KHz )
3. Sync Frequency: Prints optional synchronize frequency values. ( 1Khz 2KHz )
4. Action: Generates a digital signal which follows the required frequencies, using DAC0 while the signal consists of two parts, the synchronic part, continuos rectangular signal with the chosen frequency, and the modulation part, which is modulation of a binary number chosen with the Key-Pad. (triangle signal for the bit 1 and zero signal for the bit 0)
5. Quit: Stops the program and goes sleep mode.  
-----------------------------------
### Hardware & Connections
This project uses MSP430FG4619, 3 cables consisting of 8 wires, 9 wires, and Banana to BNC cable.
Connections are made as follows: 
* Push Buttons to P1.0-P1.3 
* IRQ to P2.0
* LCD Setup: 
     - RS to P3.5
     - RW to P3.6
     - E to P3.7
* LCD (1..7) to Port 5
* Signal Out (DAC0) to P6.6
* LEDs A to Port 9
* Calls & Rows - Key-Pad to Port 10  
