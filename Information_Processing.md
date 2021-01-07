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