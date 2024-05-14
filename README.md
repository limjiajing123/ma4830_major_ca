This project showcases a program written in C programming language that generates 4 different 
types of waveforms: sine wave, square, saw-tooth wave, and triangle wave. This program obtains 
inputs from keyboard, switches, and potentiometer to perform various function such as, changing 
the waveform, frequency and amplitude of the wave and switching the program on and off.

"Key Features"

1. Wave parameters setting – The wave parameters include waveform, amplitude, and frequency 
of the wave, which can be changed via either keyboard input or analog input. 
a. Keyboard input: The program activates the user input function by toggling the user 
input switch (SW2 – SW4). The user can change the waveform and the frequency of 
the wave by entering new value in the command prompt. Any changes to the wave 
parameters will trigger a sound alert to notify the user of the modification.
b. Analog input: The program allows flexibility in altering the amplitude of the wave. The 
user can easily adjust the amplitude by turning the potentiometer, whose resolution 
matches the amplitude scaling factor that ranges between 0x00 and 0xffff.
2. Read/write file on hard-disk/removeable disk – The program automatically savesthe waveform 
data at every timestep into an array, which is then written to a readable text file to ensure the 
repeatability of the wave. This file is stored in the same folder as the program file and can be 
copied to other directories.
3. User Interface (UI) – A user-friendly UI is programmed to guide the user step-by-step in setting 
the wave parameters. All instructions are displayed in the command prompt, and the range of 
values for each parameter is stated clearly. The program will generate an error message to 
notify the user of incorrect inputs and allow multiple attempts until the correct input is entered.
4. Real-time techniques – This program implements real-time programming techniques such as 
threading, interrupt, and mutex. Multiple threads are used to run multiple functions while 
keeping the other threads running.
5. Sounds to alert users that change has been made – While potentiometer reading or toggle 
switch is changed, an alarm sound will be emitted.

Instruction to Run the program
Before the start of the program, ensure that the main power switch (SW1) is on by switching to 
the left. The toggle switches are on when it is toggled to the left, and off when 
it is toggled to the right. When the main switch is off, the program cannot start.
The program can be started by following Command Line Arguments (CLA) usage:
./ca2 [waveform] [frequency].
