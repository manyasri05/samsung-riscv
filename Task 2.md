![p1](https://github.com/user-attachments/assets/b77902ae-ebe0-4837-baba-29a15df406ff)
Commands that are used here are:
**1. cd:** This command is used to change the current directory. In this case, the user is changing to the home directory (represented by ~).
**2. gcc add2no.c:** This command compiles a C source code file named add2no.c. The gcc command is the GNU Compiler Collection, which is used to compile C programs.
**3. ./a.out:** This executes the compiled program. The ./ part indicates that the program is located in the current directory, and a.out is the default name for the executable file created by the compiler.
The image shows a user compiling and running a simple C program that calculates the sum of two numbers in a Linux terminal environment.


![p2](https://github.com/user-attachments/assets/e85f5346-1a9a-4cae-92e1-3778efa9b008)
**riscv64-unknown-elf-gcc**
This command is a specific variant of the GNU Compiler Collection (GCC) designed for the RISC-V 64-bit architecture. Let's dissect its components:
**1.riscv64:** This part signifies that the compiler is targeting the RISC-V instruction set architecture (ISA), specifically the 64-bit version.
**2.unknown:** This indicates that the target operating system is unknown or unspecified. It's a placeholder.
**3.elf:** This refers to the Executable and Linkable Format (ELF), which is a common file format for object files and executables on many Unix-like systems.
**4.gcc:** This is the actual compiler driver. It manages the compilation process, including preprocessing, compilation, assembly, and linking.

**riscv64-unknown-elf-gcc -O1 -mabi=ilp32 -march=rv64 add2no.o add2no.c**
**1.-O1:** This flag enables optimization level 1, which performs basic optimizations like constant folding and dead code elimination.
**2.-mabi=ilp32:** This specifies the Application Binary Interface (ABI) for the target system. In this case, it's the ILP32 ABI, which uses 32-bit integers and pointers.
**3.-march=rv64:** This flag indicates that the code should be generated for the rv64 architecture, which is a 64-bit RISC-V processor.
**4.add2no.o and add2no.c:** These are the input files for the compiler. add2no.o is an object file (likely generated from a previous compilation step), and add2no.c is the source code file.

**riscv64-unknown-elf-gcc -Ofast -mabi=ilp32 -march=rv64 add2no.o add2no.c**
This command is similar to the previous one, but it uses **-Ofast** for optimization level 3, which enables aggressive optimizations that may not always preserve strict adherence to the language standard. This can result in faster code but potentially introduce unexpected behavior.


![p3](https://github.com/user-attachments/assets/5ac43832-f893-49c1-a100-ed9323bdd28f)
Understanding the Output:
**Addresses:** The first column shows the memory addresses where the corresponding machine code instructions are located.
**Hexadecimal Bytes:** The second column displays the machine code instructions in hexadecimal format.
**Assembly Instructions:** The third column shows the disassembled assembly language instructions equivalent to the machine code.
The image displays the disassembled output of an executable file, providing a low-level view of the program's instructions. This information can be useful for understanding how the program works at the machine code level, debugging issues, or optimizing performance.


![p4](https://github.com/user-attachments/assets/338be3f3-7268-49ad-9e59-febd2f6a6f33)
The image shows a user creating and compiling a simple C program to add two integers on a Linux system with a RISC-V 64-bit architecture. The steps involve writing the source code, compiling it into an object file, and checking the file information.


![p5](https://github.com/user-attachments/assets/0396a13d-e610-4908-9213-8948dc9a9066)
The image provides a low-level view of the program's instructions. This type of disassembly is useful for understanding how the program works at the machine code level, debugging issues, or optimizing performance.


![p6](https://github.com/user-attachments/assets/f03f942e-3e9c-47fc-8aa6-2f9587798a9d)
Spike is a RISC-V instruction set simulator. It allows you to run and debug RISC-V programs on your computer without needing a physical RISC-V processor. This is invaluable for development and testing purposes.
In the image, you see spike used in several instances:
**1.spike pk add2no.o**
This command starts the Spike simulator and loads the add2no.o object file into its memory.
pk is likely a configuration file or a command-line option that specifies the platform or simulation parameters for Spike.
**2.spike -d pk add2no.o**
This command also starts Spike and loads add2no.o, but with the -d flag enabled.
The -d flag enables debugging mode, allowing you to step through the program's execution, inspect registers, and examine memory.
**3.until pc @ 15184**
This is a command within the Spike debugger.
It tells Spike to run the program until the program counter (PC) reaches the address 15184. This allows you to focus on specific parts of the program's execution.
**4.reg 0 sp**
This is another debugger command.
It displays the value of register s0 (which is also known as sp for stack pointer).


![p7](https://github.com/user-attachments/assets/a1179db4-9e6d-4c0a-8a62-3e1dd9cf9e70)
The image shows a user creating, compiling, executing, and debugging a simple C program to add two integers on a Linux system with a RISC-V 64-bit architecture. The steps involve writing the source code, compiling it into an object file, checking the file information, executing the program, disassembling the executable to understand its machine code, and simulating its execution with Spike to observe its behavior at a lower level.
