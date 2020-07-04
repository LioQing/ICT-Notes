# Computer System Fundamentals

## The Components of a Computer
Main components:
- Motherboard/Main board
- Central Processor/CPU
- Display card/GPU
- Main memory
- Storage (Hard disk drive, solid state drive, etc.)
- Power supply/PSU
- DVD-ROM drive
- Floppy disk drive (_so old..._)

Peripherals - hardware devices connected to the system unit  
Include:  
- Input peripherals
- Output peripherals
- Storage peripherals
- Communication peripherals

## Central Processing Unit (CPU)
Definition:  
It executes the instructions of a program in order to process data to do tasks.  

### Arithmetic and Logic Unit (ALU)
Role:  
- Perform arithmetic operations - addition, subtraction, multiplication, division  
- Perform logical operations - comparisons with logical operators (NOT, AND, OR)
- Evaluate logic statements and return TRUE or FALSE
- Uses registers to hold data during calculations
- Results are stored in a register - _accumulator_

### Control Unit (CU)
Role:
- Keep track of sequence of instructions being processed
    1. Fetch an instruction from main memory
    2. Interpret the instruction
    3. Instruct the ALU how to perform an operation
- Monitor and coordinate all I/O operations and system units

### Rigisters

**_General Purpose Registers (GPRs)_**    
Used by instructions of assembly and machine code program
Exmaples:
- accumulator (AX)
- base register (BX)
- counter (CX)
- data register (DX)

**_Counter Registers_**  
Provide temporary memory for CU to control the operations  

**_Instruction Register (IR)_**  
Contain the instructions to be executed by the CPU

**_Program Counter (PC)_**  
Contain the memory address of the next instruction to be executed  
CPU load the next instruction addressed in PC and the control unit increase the value in PC by 1

**_Memory Address Register (MAR)_**  
Hold the memory addresses of data

**_Memory Data Register (MDR)_**  
Hold the datum (values)

*MAR and MDR facilitate the communication of the CPU with the memory through system bus

**_Status Register (SR)_**  
Contain a register that contain flag bits indicating the status after the execution of instructions

### System bus (aka bus line)
Connect the CPU and other components of the computer

Classification:
- Data bus - transfer data and instructions
- Address bus - transfer address of source or destination
- Control bus - indicate direction of transfer and coordinate timing

**_Bus width_**  
Determines the number of bits of data the computer can transmit at once

## Machine Cycle
The process of executing an instruction in a CPU

Sub-cycle:
1. Fetch - Read the instruction
2. Decode - Identify the instruction
3. Execute - Interpret the instruction and perform the operation

More detailed sub-cycle:
1. Fetch instruction
2. Decode instruction
3. Fetch operands
4. Execute instrucion
5. Store result

**_Interrpt Sub-cycle_**  
After each execution of instruction, CPU check any interruption.  
If there is interuption, CPU store the current progress, and continue with next instruction after handling the interrupt.

## Measurement of CPU Speed
### Clock Rate/Clock Frequency
Normally measured in megahurtz (MHz) or gigahertz (GHz)  
In CPU, 1 Hz = 1 clock cycle/second

### Number of Cores
Number of individual processer in a single CPU

### Number of Threads
Virtual version of cores  
Multiple lines of queue of instructions for a CPU to perform

### Word Length
The number of bits of data and instructions the CPU can handle at once

## Main Memory
Have direct access to CPU wihtout needing other I/O channels  
Installed on motherboard  

### Random Access Memory (RAM)
_Volatile_ - temporarily hold data and instructions, erased after shutdown

Classification:  
- _Dynamic RAM (DRAM)_ - lower power efficiency but higher storage capacity  
- _Static RAM (SRAM)_ - higher power efficiency but lower storage capacity

### Read-Only Memory (ROM)
_Non-volatile_ - persistent

Stores _basic input/output system (BIOS)_ for management of data transfer between input and output devices

Variance:
- Erasable programmable read-only memory (EPROM)
- Electronically erasable programmable read-only memory (EEPROM)
- More...

### Cache Memory
High-speed memory  
Stores recently used data and instructions in CPU  
Facilitate usage of requently used data and instructions  