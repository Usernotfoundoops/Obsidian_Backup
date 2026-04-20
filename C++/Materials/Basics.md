source: https://www.learncpp.com/cpp-tutorial/introduction-to-cplusplus/
1. Computer translates the C code into Machine Language Instruction which is Binary Digits (Bits)
2. Each OS has their own memory allocation to the apps that run on them and also we have to write the codes in such a way.
3. C++ (Assembly language - Human Readable) talks to CPU (Machine Language)
4. The CPU has different architecture - they process assembly codes of various length
5. x32 CPU processes 32 bit long strings, but x84 and arm64 does variable length of bits.
6. They have their own 'Machine Language' these "CPU families" is formally called the "Instruction Set Architecture" (ISA)
7. eg: for x86 CPU Architecture assembly language- `mov al, 0x61` 
8. mov=move, al=register location inside CPU, 0x61 is a hexadecimal number.
9. CPU accepts normal numbers and hexadecimal. Registers are special memories in CPU which are super fast.
10. Assembly Language -> **Assembler** -> CPU ([[Assembly Language.canvas|Assembly Language Visualization]]) 
11. C++ -> C++ COMPILER -> MACHINE LANGUAGE
12. ([[BIG IMAGE.canvas|BIG IMAGE]])
13. An **Interpreter** directly interprets the *source code* to the hardware.
14. But there's a catch
	1. The interpreter has to interpret the same code again and again if I wanna run it multiple time.
	2. I need an interpreter for every machine to run my source code.
	3. super fast
15. **Compiler** after it creates an executable, the executable can be ran on any device without the need of any outside help.