# FizzBuzz in ARM Assembly (Linux GAS Syntax)

## Overview

This project contains an ARM assembly program that implements the classic FizzBuzz challenge, counting down from 100 to 1.  
The code is written using GNU Assembler (GAS) syntax for Linux on ARM architecture.

## Features

- Prints "Fizz" for numbers divisible by 3  
- Prints "Buzz" for numbers divisible by 5  
- Prints "FizzBuzz" for numbers divisible by both 3 and 5 (i.e., 15)  
- Prints the number itself if none of the above conditions are met  
- Uses Linux system calls for output and program exit

## File

- `fizzbuzz.s` — ARM assembly source code implementing the FizzBuzz program

## Requirements

- ARM Linux environment or ARM emulator (e.g., QEMU)  
- GNU assembler (`as`) and linker (`ld`)  
- Basic knowledge of building and running assembly programs on ARM Linux

## Build and Run

To assemble, link, and run the program on an ARM Linux system or emulator:

- as -o fizzbuzz.o fizzbuzz.s
- ld -o fizzbuzz fizzbuzz.o
- ./fizzbuzz


The output will count down from 100 to 1, printing "Fizz", "Buzz", "FizzBuzz", or the number as appropriate, each on a new line.

## Notes

- The program uses the ARM Linux system call interface (`svc #0`) for writing to the console and for exiting.  
- It employs the `udiv` instruction for division, which requires ARMv7 or later.  
- The assembly uses GAS (GNU Assembler) syntax conventions.

## Author

- Suguro

- GitHub: [github.com/L1vStr34m](https://github.com/L1vStr34m)

## License

This code is provided as-is without warranty.  
Feel free to use, modify, and distribute for educational and personal projects.
