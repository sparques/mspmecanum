# MSPMECANUM

Firmware to make an MSP430 take the PWM signals output (3 axis/channel) from an RC receiver
and do the right trigonometric-magic to drive 4 mecanum (omni-direction) wheels.

I'm making this for a omni-directional skateboard-thing but no reason it won't work for a 
regular robot.

## Dependencies

I build using msp430-elf-gcc which is the mainline gcc tool chain targeting MSP430. I use the AUR package msp430-elf-gcc.

For all the necessary math, I used libfixmath, a fixed point math library implemented using 16 bit integers. https://github.com/PetteriAimonen/libfixmath

Cross compiling libfixmath for MSP430 basically worked without issue, I just had to change all the binutils from gcc to msp430-elf-gcc.


## Disclaimer

This is probably garbage code riddled with bugs and poorly implemented or misunderstood everything. 
