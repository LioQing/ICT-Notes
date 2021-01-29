# Information Systems
## Introduction
### Input-Process-Output (IPO) Cycle
- Basic division of a computer task
  1. Input: Enter data and commands
  2. Process: Process data and commands
  3. Output: Show result
### Stored Programs
- Programs: Sequence of commands
- Appliances contain small circuit board + read-only memory (ROM) to store programs
- Examples in daily life
  - automatic washing machines
  - rice cookers
  - coffee machines
### Data vs Information
Data | Information
--- | ---
raw facts | processed data
not organized | organized
no meaning | meaningful
### Data Types
**Text**
- Represented by **Character Coding Systems**
- Examples:
  - ASCII
  - Unicode
  - Big5 Code
- Text Entry Methods
  - Keyboard
  - Handwriting board
  - Optical Character Recognition (OCR)
  - Voice Recognition system

**Image**
- Types:
  - Bitmap:
    - Converted into rectangular grid of colour dots (pixels)
    - Produced by digital camera, mobile phone, scanner
  - Vector Graphics:
    - Defined by mathematical formulae

**Audio**
- Analogue signals can be captured by microphone, then turned into digital ones
- Formats:
  - WAV
  - AAC
  - MP3

**Video**
- Sequence of images in motion
  - May have sound
- Can be captured by webcam, smartphone, video camera
- Video capture card can convert analogue video to digital video

### Components of Information System
- Purpose
- Data
- Processes
- Technologies
  - Hardware: physical component related to the system
    - Input devices
    - Output devices
    - Internal hardwares (CPU, GPU, storages, motherboard)
  - Software: collection of data and instructions for the system to perform specific tasks
    - System software
    - Application software
- Personnel
  - System Analyst
    - Research, planning and implementation for end users
  - Programmer
    - Converting systems design into program code
  - Technician
    - ~~IT dog~~ Managing information systems, by doing activities such as:
      - Backup of data
      - Monitoring resource usage
  - Network Manager
    - Monitoring availability and performance
  - Data Entry Operator
    - Entering data into the system
### Information Processes
1. Data Collection
2. Organization
3. Storage
4. Processing
5. Analysis
6. Transmission
7. Presentation

### Information Age and Knowledge-based Society
3 main components:  
- Computers
  - widespread and prevalent
  - easily accessible
- Communication networks
  - high transmission speed
  - wide area coverage
  - low cost
- People
  - can handle large amount of information
  - can deteremine the information required
  - can use relevant information to complete tasks
  - can convert information from one form to another
  - use information ethically and legally
  - live with a style of lifelong learning

## Data Organization and Data Control

### Data Input Error
Error | Source of Error
--- | ---
data srouce error | data source providers provide incorrect data
transcription error | data is read of typed in incorrectly
transposition error | 2 consecutive digits are swapped

**garbage-in-garbage-out (GIGO)**  
def: erroneous data produces inaccurate information

### Data Control
**data validation**  
def: the process of comparing data with a set of rules or values  
aim: to make sure the data is reasonable and valid  

Validity check | Function | Example
--- | --- | ---
field presence check | is present in a field | student number in student record
field length check | length (no. of characters/digits) is within a range or is correct | number of students > 0 or telephone number = 8 digits
range check | is within pre-determined range | mark of a test from 0 to 100
fixed value check | is one of the values in a pre-defined list | gender of a person be either 'Male' or 'Female'
format check | follows a known format/pattern | e-mail address consists of (user name) + '@' + (domain name)
type check | is of correct data type | test mark must be number, not letters
check digit | check digit found by using a math formula on a numerical data | usage of **parity check** on ID card number

### Error Detection (Extra)
**check the reliability** of the digital data delivered

Types:
- Repetition codes
 	- sends the data multiple times
- Vertical redundancy check (**VRC**) / **Parity check**
 	- **odd parity**
 	- **even parity**
- Longitudinal redundancy check (**LRC**) / 2-D parity check
 	- data arranged in 2D table with fixed rows and columns
- **Checksum**
 	- modular arithmetic sum of data over a fixed word length
- Cyclic redundancy check (**CRC**)
 	- based on remainder of a polynomial function

### Data Verification
def: the control to check whether the inputted data matches that in the source document  

- input data twice
	- by same person
	- e.g. e-mail address or password when creating online account
- double data entry
	- by different person

### Data Hierarchy
top to bottom level:
1. database
	- collection of interrelated tables
	- e.g. database of a school library (containing tables for student, book, loan records)
2. table
	- collection of similar records
	- each row is a record
	- each column is a field
3. record
	- collection of fields
	- e.g. personal records of students
4. field
	- combination of characters, meaningful information
	- e.g. telephone number, mailing address, monethly income, marital status
5. data
	- characters

### Database Mangment System (DBMS)  

features/functions:
- organize and manage data structure
- allowed to access, create, organize, retrieve, control data
- data can be integrated and presented

advantages:
- avoid uncontrolled data redundancy and preventing inconsistency
- program-data independence (program extract data from DBMS)
- flexible access to shared data
- centralized control of data

### File Access Modes
- sequential access mode
	- data are stored and accessed one by one by read/write head
	- application
		- for records that will be processed periodically
		- e.g. payroll processing, backup and recovery of database
	- example devices
		- magnetic tape
- direct access mode
	- data are stored and accessed directly on a 2D plate by read/write head
	- application
		- for applications needed for immediate and direct access to data
		- e.g. airline reservation, online banking transaction, secondary storage for OS
	- example devices
		- floppy disks
		- optical disks (DVD-RAM, CD-RW)

## Data Representation

### Number Systems
commonly used:
- denary (base 10)
- binary (base 2)
- hexadecimal (base 16)
  - 10 to 15 = A to F

conversion trick:  
**binary to hexadecimal** (or reverse for hex to bin)
1. 10011011<sub>2</sub>
2. 1\*8+0\*4+0*2+1\*1 ***+*** 1\*8+0\*4+1\*2+1\*1
3. 9 ***+*** B(11)
4. 9B<sub>16</sub>

### Number Representation in Computer System

units:
- Bit
  - abbr: b
  - size: 2 states (1 or 0)
  - def: the basic unit of a binary digit
- Byte
  - abbr: B
  - size: 8 b
- Kilobyte
  - abbr: KB
  - size: 2<sup>10</sup> B = 1,024 B
- Megabyte
  - abbr: MB
  - size: 2<sup>20</sup> B = 1,024 KB = 1,048,576 B
- Gigabyte
  - abbr: GB
  - size: 2<sup>30</sup> B = 1,024 MB ≈ 1 billion B
- Terabyte
  - abbr: TB
  - size: 2<sup>40</sup> B = 1,024 GB ≈ 1 trillion B

**representation of unsigned binary integer**  
word length | range of value
--- | ---
4-bit | 0<sub>10</sub> to 15<sub>10</sub>
8-bit | 0<sub>10</sub> to 255<sub>10</sub>
16-bit | 0<sub>10</sub> to 65,536<sub>10</sub>
24-bit | 0<sub>10</sub> to 16,777,216<sub>10</sub>
<br>

**sign-and-magnitude**  
the sign bit (leftmost) is to specify the sign  
i.e. 0 is positive, 1 is negative

word length | range of value
--- | ---
4-bit | -7<sub>10</sub> to 7<sub>10</sub>
8-bit | -127<sub>10</sub> to 127<sub>10</sub>
16-bit | -32,767<sub>10</sub> to 32,767<sub>10</sub>
24-bit | -8,388,607<sub>10</sub> to 8,388,607<sub>10</sub>
<br>

**two's complement**  
widely used in computers  
such that value of 0 won't be represented by 2 numbers (like in sign-and-magnitude)  

convert from binary integer to two's complement:  
1. convert the positive binary integer to one's complement
	- flip all digits (1 to 0, 0 to 1)
2. add 1 to the one's complement

### Addition and Subtraction
all number systems have the same way as denary addition and subtraction (including two's complement)  

**overflow error**  
def: when 2 numbers are added and subtracted, it exceeds the range to store the result  
example: 8-bit unsigned integer range from 0<sub>10</sub> to 255<sub>10</sub>, when a number results in more than this value is calculated, overflow error occurs  

two's complement overflow error:  
when number calculated has the opposite sign as the 2 added or subtracted numbers  

### Character Coding Systems

**American Standard Code for Information Interchange (ASCII)**  
size: 7 bits (2<sup>7</sup> different characters)  
table: http://www.asciitable.com/

**Chinese Character Coding Systems**  
common character coding systems:
- Big5
	- used for traditional chinese
	- size: 2 B
	- used in HK, Macau, TW
- Guo Biao (GB)
	- used for simplified chinese
	- size: 2 B
- **Unicode**
	- used for all existing languages in the world
	- size: 1 B to 4 B
	- represented by **code points** (variable in length)
	- commonly used characters are in the front of the code table
	- used as international standard

### Graphics

**bitmap/raster graphics**  
def: 
- resolution - number of rows and columns of pixels
	- unit: pixel per inch (ppi)
	- screen display: 72 to 95 ppi
	- photograph printing: 200 ppi to 400 ppi
- colour depth - size of storage to represent colour in each pixels  
	- unit: bits
	- common colour depth: 1, 8, 16, 24 bits

file size = resolution × colour depth = height × width × colour depth  

formats:  
- jpg/jpeg
- png
- gif
- bmp

**vector graphics**  
def:
- vector objects
	- defined by mathematical formulae

usage:
- logo
- banner
- line art
- detailed drawings in deisgn works (e.g. architectural design)

formats:
- svg
- pdf
- ai

**comparison**  
<empty/> | bitmap grpahics | vector graphics
--- | --- | ---
file size | larger | smaller
factors of file size | resolution & colour depth | complexity of objects
resolution | fixed | independent
edit | pixels | shapes and lines
usage | computer display, photography | logo, design works, line art
advantage | directly digitized from camera | zooming in does not cause quality downgrade

### Audio

def:
- sample size / bit resolution - number of bits taken in each sample  
	- unit: bit
	- general size: 8-bit, 16-bit, 24-bit, 32-bit
- sampling rate - number of sample taken per unit time
	- unit: hertz (Hz) - per second
	- general size: 11,025 Hz, 22,050 Hz, 44,100 Hz, 96,000 Hz
- duration - total time length  
	- unit: second
- no. of channels
	- mono audio = audio of 1 channel
	- stereo audio = audio of 2 channels

audio | sample size | sampling rate
--- | --- | ---
voice over telephone | 8-bit | 11,025 Hz
FM broadcast | 16-bit | 22,050 Hz
Compact disc | 16-bit | 44,100 Hz
DVD | 24-bit | 96,000 Hz
music | 16-bit | 44,100 Hz
movie & video | 16-bit | 48,000 Hz

file size = sample size × sampling rate × duration × no. of channels

formats:
- mp3
- wav

*extra*
44.1 kHz & 48 kHz are the most common sampling rate
reason: https://www.youtube.com/watch?v=fZzMXdxbOes

### Video
mechanism:
a sequence of images played at high speed to give the sense of motion and continuity

def:
- frame size
	- unit: {no. of pixels} × {no. of pixels}
	- dimension of one frame in pixels
- frame rate
	- unit: frames per second (fps)
	- number of frame displayed per unit time
- duration
	- unit: second
	- play time of the video
- colour depth
	- unit: bit
	- size of storage to represent colour of a pixel

formats:
- avi
- mp4
- mpeg-1
- mpeg-2
- wmv

## Analogue Data & Digital Data

<empty/> | analogue data | digital data
--- | --- | ---
representation & measurement | continuous | discrete
physical size | large | small
life-time | short | long
transmission efficiency | high rate of error | low rate of error
accuracy | depends on sampling technique | low
absolute replication | nearly impossible as data is lost in the process | possible, error-free and easy
mode of access | mostly sequential access | depends (direct access is possible)
data analysis | difficult to search, analyze, reconstruct | easy to be reused and processed by computer

## Conversion between Analogue Data & Digital Data


**digitization**  
def: the process of converting analogue data to digital data

steps:
1. sampling
	- obtaining the sample data from analogue signal every fixed time interval  
2. quantization
	- converting attribute of each sample data into digital code using predefined scale