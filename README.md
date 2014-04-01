ECE281_CE4
==========

PRISM Assembly Language for Starters

__*PROGRAM DESCRIPTIONS*__


_Part A_

In part A, the program was to store $9 in $B0, $8 in $C4, and $B in $CB. To go about this, LDAI instructions loaded the specific operand into the accumulator, and immediately after the STA instruction stored the number loaded into the accumulator into the specific operand address specified by a pointer variable. Finally the JMP instruction looped infinitely back to itself.


_Part B_

In part B, the program was to load a value from the $B0 operand adress to the accumulator, then add the same value to the accumalator. Then the program was to subtract 4 from the accumulator, and finally outputting the accumulator value to the Output Port 2. Using the LDAD instruction and a pointer to a specific operand address, I loaded the value stored in the operand address into the accumulator, then added the same value from the operand address using ADDD and the pointer. Then to subtract 4, I added operand C to the accumulator using ADDI. Again I used the infinite loop at the end of the program to keep the computer from crashing.


_Part C_

In part C, the program was to load a value from input port, then output the value into Output Port 0, then the value minus 1 in Ouput Port 1, and the value minus 2 in Ouput Port 2. All three Ouput Ports decrement in order continuously. First, the IN instruction was called to get the value from the input port. The the value from the accumulator was outputted for each using OUT, and the specific output port number as the operand. To make each output one less than the other, I used ADDI with the operand F, because the value was still stored in the accumulator. Then after decrementing by one, I added one to the accumulator using ADDI also, and used the JMP loop to loop back to the first ouput port that the accumulator was outputted to.


**All programs reach target end for +1 bonus each, and +4 for approval by Capt Silva for finding legitimate error.
