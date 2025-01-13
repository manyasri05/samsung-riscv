The first snapshot says:
           1.The sum variable is initialized to 0.
           2.The for loop iterates from 1 to 5, adding each number to the sum variable.
           3.The final value of sum is printed to the console.
# samsung-riscv![WhatsApp Image 2025-01-07 at 15 28 34_799a344a](https://github.com/user-attachments/assets/1b99ef1d-2ab1-45a9-a8b0-3ff8d8d5eadc)
The second snapshot says:
steps-
           1.Compilation:gcc sumiton.c -o sumiton.o: This command compiles the C source code (sumiton.c) into an object file (sumiton.o). The object file contains the machine code instructions that the computer can understand.
           2.Linking:riscv64-unknown-elf-gcc -o1 -mabi=lp64 -march=rv64 sumiton.o sumiton.c: This command links the object file (sumiton.o) with the C source code (sumiton.c) to create the final executable file (sumiton). The flags -o1, -mabi=lp64, and -march=rv64 are likely compiler optimization and architecture-specific options.
           3.Verification:ls -ltr sumiton.o: This command lists the file information for the object file (sumiton.o). It shows the file permissions, owner, size, and modification time.
![WhatsApp Image 2025-01-07 at 15 29 07_0b399364](https://github.com/user-attachments/assets/5e501b80-ab96-42a1-becf-1bd4aad65fd7)
The third snapshot says:
           1.Assembly Language: The output is in assembly language, a low-level programming language that directly interacts with the computer's hardware.
           2.Disassembly: The process of converting machine code (binary instructions) back into human-readable assembly language is called disassembly.
           3.Memory Addresses: The left-hand side shows memory addresses where the corresponding assembly instructions are located.
           4.Instructions: The right-hand side displays the assembly instructions themselves.
![WhatsApp Image 2025-01-07 at 15 29 31_100738bb](https://github.com/user-attachments/assets/384960de-a2a9-4a35-a47a-1f789d5bf43e)
