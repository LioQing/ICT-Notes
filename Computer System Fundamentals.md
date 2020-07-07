# Computer System Fundamentals

## The System Unit of a Computer System
This chapter talks about what and how main components of a computer there are and works

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
4. Execute instruction
5. Store result
6. Check interruption

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

## Input and Output Devices
This chapter talks about devices that are connected to the computer for input and output purpose

## Input Devices
Allow user to enter data into a computer and convert the data into a computer-readable form

### Keyboards
Allow user to enter data by pressing keys  
Converts keystrokes into corresponding eletrical signal for computer to read  

### Pointing Devices
Allow user to control a cursor/pointer on a graphical user interface (GUI) and trigger action  

**_Mouse (Plural: Mice)_**  
Multidirectional mechanism to register its motion => control pointer  
- Mechanical mouse - has a ball on its underside, track the direction of the ball's movement
- Optical mouse - has an optical sensor to detect its movement more accurately
- Buttons on top

**_Trackball_**  
Roll the ball with finger to control the pointer
- The base remain stationary
- Buttons next to the ball

**_Touchpad_**  
Drag finger on the touch-sensitive plate to move the pointer
- Usually found on notebook computer
- Tapping the pad same as clicking a button on a mouse

**_Trackpoint_**  
Push the pressure-sensitive stick for moving the pointer in the direction it is pushed  
- Usually found on notebook computer

**_Joystick_**  
Move the vertical lever to control the pointer
- Designed for playing computer games
- Trigger buttons

**_Touch Screen_**  
Use finger or stylus touches by pressing and dragging icons or figures on a screen and the touch-sensitive layer sends an electical signal to the computer to move the pointer and perform action
- Used in informations kiosk
- Used in smart phone
- Used in handheld game consoles
- Used in notebook computer

**_Digitizing Tablet_**  
The tablet detect the movement and pressure of a pen-like stylus and convert it into electrical signal  
- Allow user to draw and sketch directly
- Widely used in graphic design and engineering

**_Handwriting Board_**  
Working mechanism similar to digitizing tablet with a pressure-sensitive board and a pen-like stylus
- Designed for Chinese character input
- Must work with character recognition software

### Scanner
Projects the light onto an object (paper, slide), capture the reflected light and interpret the pattern and colours  
Factors for its quality: 
- Resolution - the sharpness of the picture - measured in dots per inch (dpi)
- Colour depth/bit depth - amount of colours to represent each dot
- Accuracy - the image's likeness, in terms of colour and shape to original object

*Can be used with _optical character recognition (OCR) software_ to convert text into editable file

### Optical Reader
Read predetermined characters, marks, or codes and translate into digital data for computer to read

Bar Code Reader
- Increase the accuracy and efficiency of data entry
- Process is done instantly and accurately
- Commonely used in libraries on all books

Optical Mark Reader
- Used with optical mark recognition (OMR) software
- Commonly used for multiple choice answer sheet, questionnaires, lottery tickets, etc.

### Microphone
Record sounds as eletrical signals to convert into sound
- Connected to sound card
- Can be used with speech recognition software

### Digital Camera and Digiti Video Camera (DC)
Use light-sensitive processor to capture scense to turn them into digital images
- Image quality depends on compression ratio, file format, resolution
- Usually has a screen to make the scene immediately be viewable to the user
- Special type of DC is web cam - connected to the computer
- Smart phones have built-in cameras for photo taking and video recording

## Output Devices
Hardwares that translate computer processes and information into forms that human can comprehend

### Visual Display Unit (VDU) && Monitor
View computers output on a screen

Classification:
- Cathode ray tube (CRT) monitor
- Liquid crystal display (LCD) monitor  

Quality determined by:
- Resolution - number of pixels a monitor can display
- Dot pitch - vertical distance between each pixels on a screen
- Contrast ratio - the difference in light intensity between the brightest white and darkest black
- Refresh rate - the number of times the screen refresh per second (Hz)

### Speakers
Convert audio signals of a computer into sounds.  
Connected to sound card which convert digital audio signal into analogue signal for output

### Printers

**_Dot-matrix Printer_**  
- Ideal for printing multi-part forms
- Low printing cost

**_Inkjet Printers_**  
- Cheaper than laser
- Use cartridge 
- Expensive printing cost

**_Laser Printers_**  
- High resolution at high speed
- Medium printing cost

**_Thermal Printers_**
- Commonly used in point-of-sale
- Use thermal paper to heat to turn black
- Black and white

**_Plotter_**
- High-quality
- Large-format printouts

### Multifunction Printers
Includes a variety of functions:  
- a printer
- a scanner
- a photocopier
- a fax machine
- a telephone
- suitable for small office home office (SOHO)

### Video Projectors  
Project the computer display onto a large screen by high light intensity light bulbs and a set of optical lens  

Classification: 
- Liquid crystal display (LCD) projector
- Digital light process (DLP) projector

## Daily Application
- Point-of-sale (POS) Terminals 
- Cheque Deposit Machine
- Small Office Home Office (SOHO)
- Conference Room

## Secondary Storage Devices
Also called backing storage
- store data, operating system, application software
- non-volatile

## The Speed of a Secondary Storage Device
- Access time  
    - Average time taken to search and read the required data
    - Measured in millisecond (ms)
- Data transfer rate
    - The amound of data can be transferred between main memory and a storage device per second
    - Measured in megabyte per second (MBps)

## Storage Capacity
The maximimum amount of data can be stored in a storage medium  
Units in ascending order:  
(increasing with 1024 of the previous unit)
- Byte - B
- Kilobyte - KB
- Megabyte - MB
- Gigabyte - GB
- Terabyte - TB
- Petabyte - PB

## Categories of Storage Devices
Categories:
- Magnetic storage devices
- Optical storage devices
- Others (e.g. memory cards, USB flash drives)

Parameters:
- Price - price per volume
- Capacity - storage capacity
- Speed - access time and data transfer rate
- Lifespan - rewritability
- Durability - physical durability
- Portability - portability
- Popularity - popularity as of 2020
- Usage - common usage

## Magnetic Storage Devices
- Floppy disks
    - Price - cheap
    - Capacity - very low (<= 1.44MB)
    - Speed - slow
    - Lifespan - short
    - Durability - weak
    - Portability - high
    - Popularity - non
    - Usage - replaced by USB flash drives
- Hard disks
    - Price - medium
    - Capacity - very large (~2TB) (still improving nowadays)
    - Speed - fast
    - Lifespan - long
    - Durability - medium
    - Portability - low
    - Popularity - very popular
    - Usage - computer storage
- Magnetic tape
    - Price - cheapest
    - Capacity - very large (varies, up to 170 TB)
    - Speed - slow
    - Lifespan - very long
    - Durability - low
    - Portability - medium
    - Popularity - medium (mainly in businesses)
    - Usage - backups

## Optical Storage Devices
- Compact Disc Read-Only Memory (CD-ROM)
    - Price - medium
    - Capacity - low (up to 750MB)
    - Speed - very slow
    - Lifespan -
    - Durability -
    - Portability -
    - Popularity -
    - Usage - audio or program files
- Digital Versatile Disc (DVD)
    - Price - medium
    - Capacity - low (4.7GB for single layer, 8.5GB for double)
    - Speed - slow
    - Lifespan -
    - Durability -
    - Portability -
    - Popularity -
    - Usage - video or substantial amount of program files
- HD DVD and Blu-ray Disc
    - Price - 
    - Capacity -
    - Speed - medium
    - Lifespan -
    - Durability -
    - Portability -
    - Popularity -
    - Usage - 
- Solid State Drive (SSD)
    - Price - high
    - Capacity -
    - Speed - very fast
    - Lifespan - long
    - Durability - high
    - Portability -
    - Popularity - very popular
    - Usage - computer storage (small storage)

## Others
- Magneto-optical (MO) Disks
    - Price - 
    - Capacity - medium 
    - Speed - 
    - Lifespan - 
    - Durability - 
    - Portability -
    - Popularity - 
    - Usage - replaced by DVD
- Memory Cards
    - Price - 
    - Capacity - high (from a few MB up to 64GB)
    - Speed - 
    - Lifespan - 
    - Durability - 
    - Portability -
    - Popularity - 
    - Usage - mobile devices (smart phone, portable game console, digital camera, notebook computer)
- USB Flash Drives
    - Price - 
    - Capacity - high (about 2GB - 128GB)
    - Speed - 
    - Lifespan - 
    - Durability - 
    - Portability -
    - Popularity - very popular
    - Usage - as portable storage device

## Network Storage
Compared to local hard drives:
- Pros
    - facilitate sharing of information
    - facilitate storage management such as backups
- Cons
    - requires a network connection

Forms:
- a storage device directly attached to a file server in a network
- a storage system connected to a network, network-attached storage (NAS) and storage area network (SAN)
- remote computer for the storage, such as Internet hard drives (e.g. Google Drive)

## System Software and Application Software

## System Software
- Operating system - manage resources and other application softwares can run on it
- Utility program - perform security tasks, data protection and resource optimization
- Driver program - allow communication between hardware devices and the computer system

**_Features_**
- single-user <=> multi-user
- single-tasking <=> multi-tasking
- multi-processing

## Operating Systems

Operating system's functions:
- device configuration
- memory management
- interface platform
- file management
- network communication management

Categories:
- Network operating system
    - Run on network servers that centralize storage, communication channels, peripheral devices, sharing services, etc.
    - E.g. UNIX, Microsoft Windows NT, Microsoft Windows Server 2008, Linux
- Desktop operating system
    - Run on standalone desktop and notebook computers
    - High hardware expandability
    - High software compatibility
    - E.g. DOS, Microsoft Windows XP/Vista/7/8/10, Mac OS X
- Mobile operating system
    - Run on personal digital assistants (PDAs), smart phone, wireless communication devices, small computing devices
    - E.g. Palm OS, Microsoft Windows Mobile, Android, iOS

Comparison table of various common OSes:  
</empty> | DOS | Microsoft Windows | Mac OS | UNIX | Linux | Palm OS/Microsoft Windows Mobile/Android/iOS
--- | --- | --- | --- | --- | --- | ---
Number of users | Single-user | Desktop OS: single-user; Network OS: multi-user | Signel-user | Multi-user | Multi-user | Single-user
Single/multi-tasking | Single-tasking | Multi-tasking | Multi-tasking | Multi-tasking | Multi-tasking | Multi-tasking
User interface | CLI | GUI | GUI | CLI & GUI | CLI & GUI | GUI
Category | Desktop OS | Desktop OS/Network OS | Desktop OS | Network OS | Network OS | Mobile OS  

## Utility Program
desgiend to enhance an OS by providing ways for user to protect files, manage resources and refine system

- backup utility
- data recovery utility
- file manager
- anti-virus software
- program uninstaller
- file comperssion utility
- disk scanning program
- disk refragmenter
- system monitoring software
- more...

## Driver Programs
Allow some peripheral devices to communicate with the computer  
Examples of peripheral devices:
- printer
- scanner
- external modem

## Application Software (aka Integrated Software)
Enables users to perform specific tasks  
Cannot run on computer without an operating system
Classification:
- productivity software
- communication software
- multimedia software
- entertainment software
- education software

***Productivity Software***  
To perform tasks needed in school or workplace
- Word processor - for word processing
    - Microsoft Word
    - OpenOffice.org Writer
- Spreadsheet - for mathematical manipulation
    - Microsoft Excel
    - OpenOffice.org Calc
- Presentation software - for presentation
    - Microsoft PowerPoint
    - OpenOffice.org Impress
- Database software - for database management
    - Microsoft Access
    - OpenOffice.org Base
    - MySQL
- Finance software - for financial management
    - Microsoft Money
    - Quicken

***Communication Software***  
Enables users to communicate or share information with others

- E-mail program
    - Microsoft Outlook
    - Microsoft Live Mail
- Web browser
    - Internet Explorer (DEAD)
    - Microsoft Edge
    - Google Chrome
    - Mozilla Firefox
- File transfer protocal (FTP) program
    - WS FTP
    - FireFTP
- Instant messaging program
    - Yahoo!Messenger
    - Skype
    - Discord

***Multimedia Software***  
Enables users to create and manage multimedia files

- Graphics software
    - Adobe Photoshop
    - GIMP
    - Paint.NET
- Audio editing software
    - Adobe Audicity
    - Anvil Studio
    - FL Studio
- Video editing software
    - Adobe Premiere
    - Window Movie Maker (not supported anymore)
    - iMovie
- Web authoring software
    - Adobe Dreamweaver
    - Microsoft Expression Web
- Computer-aided design (CAD) software
    - Blender
    - NX
    - Caddie
    - AutoCAD
- Media management software
    - Windows Media Center
    - Google Picasa

***Entertainment Software***  
Enables users to play computer games and run multimedia files such as movies

- Game
    - Wolfenstein 3D
    - Counter-Strike
    - StarCraft
    - World of Warcraft
- Multimedia program
    - VLC media player
    - Windows Media Player
    - QuickTime Player

***Education Software***  
As a tool to facilitate the learning process of users

- Electronic dictionary
    - Longman Dictionary of Contemporary English
- Encyclopedia and reference program
    - Encyclopedia Britannica
    - Microsoft Encarta
- Self-learning program
    - Microsoft Math
    - Animated Beginning Phonics 1.0

## Computer Systems
### Classification of Computers
- Personal Computers
    - Desktop Computers
        - Workstations
    - Notebook Computers (aka laptop computer)
    - Handheld Computers (What is this...)
    - Network Computers
        - E.g. POS terminal
- Mainframe Computers
- Supercomputers

Comparison between desktop computers and notebook computers:
</empty> | Desktop Computers | Notebook Computers
---|---|---
Ability of extension | Higher | Lower
Cost (with similar specs) | Lower | Higher
Portability | Non | High
Power consumption | Higher | Lower

Almost every aspects of a computer:  
personal computer < mainframe computer < supercomputer

***Applications***
- Personal computer
    - Office application
    - Internet access
    - Entertainment
- Mainframe computer
    - Database management
    - Web hosting
    - File management (of an organization)
- Supercomputer
    - Tailored program for scientific research
    - Weather forecasting
    - Military operation controls

### Characteristics of Computer Systems
Classified by modes of operation, the number of users, the ways of organization of networked computers  

