# Software Development
## Compulsory

### Logical Operations

Transformation of logical expressions:  
not (A and B) -> not A or not B  
not (A or B) -> not A and not B  
not (not A) -> A  

example: 
not (A and (B or C)) -> not A or not (B or C) -> not A or not B and not C  
not (A or (B and C)) -> not A and not (B and C) -> not A and (not B or not C)  
not (A and B and C) -> not A or not B or not C  

### Pseudo Code

> Note: To shorten the code, `{V}`, `s` and `e` has been used to represent `{VARIABLE}`, `start` and `end` respectively

| Operators / Keyword                           | C/C++                                          | Pascal                                        | Python                         | Description                 |
|-----------------------------------------------|------------------------------------------------|-----------------------------------------------|--------------------------------|-----------------------------|
| `<-`                                          | `=`                                            | `:=`                                          | `=`                            | Assign value to a variable  |
| `INPUT {V}`                                   | `scanf(%{V_TYPE}, {V})`                        | `read({V})`                                   | `{V} = input()`                | Get input value to variable |
| `OUTPUT {V}`                                  | `printf("%{V_TYPE}", {V})`                     | `write({V})`                                  | `print({V})`                   | Output variable value       |
| `FOR {V} FROM s TO e DO`                      | `for(int {V} = s; s <= e; s++)`                | `for {V} := s to e do`                        | `for {v} in range (s, e + 1):` | For loop                    |
| `WHILE {CONDITION} DO`                        | `while {CONDITION}`                            | `while {CONDITION} do`                        | `while {CONDITION}:`           | While loop                  |
| <pre>REPEAT<br>...<br>UNTIL {CONDITION}</pre> | <pre>do{<br>    ...<br>}while(!{CONDITION})</pre> | <pre>REPEAT<br>...<br>UNTIL {CONDITION}</pre> | **DOES NOT EXISTS**            | Repeat until loop |
| `IF {CONDITION} THEN`                         | `if ({CONDITION}){...}`                        | `if {CONDITION} then`                         | `if {CONDITION}:`              | If case                     |

### Flowchart

| Symbol                                                         | Name               | Description                                                                                   |
|----------------------------------------------------------------|--------------------|-----------------------------------------------------------------------------------------------|
| ![arrow](assets/flowchart/arrow.png)                           | Flow Line          | Indicates the direction of process flow                                                       |
| ![oval](assets/flowchart/oval.png)                             | Terminal           | Indicates the beginning and ending of a program or sub-process.                               |
| ![rectangle](assets/flowchart/rectangle.png)                   | Process            | Indicates the process of changing a variable's value, excluding input the value to a variable |
| ![parallelogram](assets/flowchart/parallelogram.png)           | Input/Output       | Indicates the input/output process                                                            |
| ![rhombus](assets/flowchart/rhombus.png)                       | Decision           | Indicates a decision, decision block is used when preforming a **loop** or a **if case**      |
| ![predefined process](assets/flowchart/predefined_process.png) | Predefined Process | Indicates name of a process which is defined elsewhere, you may think it as a subprogram      |

## Elective D

> All the content below is related to elective D module

## Programming Languages Generations

### Generation 

Name: X Generation Language = XGL (X is a number)  

### First Gen - Machine language  

Machine language = machine code  
Properties:  

* Binary  
* **Machine dependent**  

### Second Gen - Assembly language  

Instructions are called __mnemonic__  
Code example:  

``` 
ADD dest, src  
```

`ADD` : opcode  
`dest` and `src` : operand  

Properties:  

* __Directly control CPU__  

### Third Gen - High level programming language  

Examples:  

* C/C++  
* Pascal  
* BASIC  
* Ada  
* Fortran  

Properties (Advantage):  

* Closer to human language and more like English  
* __Machine independency__  

Properties (Disadvantage):  

* Loss of direct control of CPU and memory address => less efficient  

### Fourth Gen  

Examples:  
Structured Query Language (SQL)  
Cascading Style Sheets (CSS)  

### Fifth Gen  

Artificial Intelligent (AI)  

## Programming Paradigm

Language classification by pattern/model

### Procedural/Imperative  

Focus on ‘how’ the goal should be reached  
By using control statements to direct flows to change state (data) of the program  
Usually for general-purpose

Examples:  

* C  
* BASIC  
* Pascal  

### Declarative  

Focus on ‘what’ the goal is  
Commonly used for domain-specific purposes

#### Logic Programming Language:  

Commonly used in AI  
Most well-known: Prolog (Programming in Logic)  
2 type of clause: facts and rules  

#### Query Programming Language:  

Commonly used in database management system (DBMS)  
Most well-known: Structured Query Language (SQL/SEQUEL)  
Examples:  

* Oracle  
* Microsoft Access  

### Object-oriented Programming(OOP)  

Examples:  

* C++  
* Java  
* Python  
* JavaScript  

#### Objects and Classes

Object consist of multiple type of data that define properties of an object  
Consist of functions (methods) that define the behavior of an object

Class is template for object, so that multiple objects of the same properties (attributes) and functions (behaviors) can be created and stored  

Objects and Classes allows better __reusability__ of the codes in the program  
Objects and Classes have the following 3 features:

#### Encapsulation:  

Advantage: __access control__ (setter/getter)  
Explain:  

* Public variable (accessable from outside the class)
* Private variable (only accessable from inside the class)

#### Inheritance:  

Advantage: __reusability__  
Explain:  

* Inheritance/extend (functions or variables can be inherited to other classes)  

#### Polymorphism:  

Advantage: __reusability__  
Explain:  
Same class can have different forms in the form of subclass

### Criteria of Selecting a Language for a Specific Program

* Platform to be used
* Nature and size of the problem
* Program execution efficiency and hardware control
* Portability
* Program development time

following are from 2017 2D section:
* Scale and modularity
* Reusability
* Portability
* Execution efficiency
* Functional strength
* Readability
* Utility libraries and development tools
* End-user interaction
* Familiarity
* Cost

_Revision with examples is better!_  
_Use the following **besttest** examples from the almighty Comp Soc!_  
_https://github.com/spc-comp-soc/spc-cs-db_

## The Generation of Executable Files

High level languages are compiled into machine code for the computer to execute.  
Computer have a series of action to compile a program developed in programming language such as C/C++, Pascal, Java, etc.  

### Program Code Generation

-> (arrow): compile-time process  
=> (arrow): run-time process   

Program development  
-> Source code (.c)  
-> Compile (stop if compile-time error occurs)  
-> Object code  
-> Linker (links program libraries & shared libraries)  
-> Executable code (.exe) (in hard disks)  
=> Loader (operating system) (loads dynamic link libraries)  
=> Executable code (in main memory)  
=> CPU (return if run-time error occurs)  
=> Program result

### Linkers and Loaders

Object code contains reference to external libraries.  
Linker is required to build a fully executable code from object code.  
Ready-to-use libraries are called __library routines__.  

***Dynamic Link Libraries (DLL)***  
DLL are not copied into the executable code.  
They are located from the disk, and mapped into the memory space of the program during run-time by __loader__.  

In C, referencing a library (e.g. some_library) is done as follows:  
 `#include <some_library>`

### Translators

translate source code into object code

***Assembler***  
translate assembly language into machine code

In high level programming language, there are 2 translators: 

***Interpreters***  
translate source code into machine code and execute  
Examples: python, javascript

***Compilers***  
compile source code into object code for linker to link libraries into executable  
Examples: C/C++, Java

table of comparison:

| </empty>                                         | Interpreters                                            | Compilers                                                                                                                                                   |
|--------------------------------------------------|---------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Mode of translation                              | One statement a time                                    | One program a time                                                                                                                                          |
| Mode of program execution                        | One translated statement at a time                      | Complete translated program                                                                                                                                 |
| Presence of object code                          | No                                                      | Yes                                                                                                                                                         |
| Independent program execution without translator | No                                                      | Yes                                                                                                                                                         |
| Error detection                                  | Errors are returned during translation of the statement | Errors such as syntax errors are returned during compilation (compile-time error); other undetectable errors are returned during execution (run-time error) |

## System

Definition of system:  
a system of interacting elements that work as a whole to accomplish specific tasks or functions  
E.g. alveolar cells (cells) => air sac/ alveoli (tissues) => lung (organ) => respiratory system (system) => respirate (function)  

### Characteristics 

Elements are interrelated and interdependent  

### Boundary and Environment  

Scope tells what the system is supposed to achieve upon its completion in accordance with the user needs  

### Interface  

Definition:   
The communication boundary between two entities  

System interface of an information system:  
Allows information flow between a system and its environment  
E.g. input and output devices  

### Subsystem/Processes  

Definition of subsystems:  
Smaller system elements of a system  

### System Status  

Storage to store them  
System may react differently to the same input depending on its current status  

### Information System  

Definition of information system:  
A system that comprises people, machines, and/or methods organized to collect, process, transmit, and disseminate data the represent user information  

Made up of elements, defined with a clear boundary, equipped with interface    

Characteristics:  

* Has its users  
* Has its purpose and some functions to offer  
* Has a boundary and well defined scope  
* May be composed of some sub-systems, their purpose are also clearly defined  
* Subsystems within the same information system interact  

### Developing a New System  

3 solutions:  

* Software package  
* In-house development  
* Outsourcing  

Factors on deciding:  

* Suitable package exists or not  
* Has suitable staff to develop or not  
* Cost-effective to develop in-house or not  
* Has reliable and experienced developers to take up outsourced project or not  
* Has suitable staff to administer the software or not  
* Project budget  
* More...  

### System Development Life Cycle (SDLC)  

Definition of SDLC:  
Conceptual model for development of an information system  
E.g. waterfall model, rapid application development (RAD)  

### The Waterfall Model  

Characteristics:  

* Sequential and linear  
* Phases with well-defined beginning and end points  
* Distinctive goals and end with deliverables  
* No turning back to a previous phase  

Procedures:

1. Analysis  
2. Design  
3. Implementation  
4. Maintenance  

## Phases of SDLC and Project Initiation

1. Systems Analysis
2. Systems Design
3. Systems Implementation
4. Systems Conversion and Maintenance
5. Documentation

Solutions:

* Off-the-shelf softwares package => software packages
* In-house team => in-house development
* Hire a service provider => outsourcing

### Systems Analysis

#### Identifying users’ requirements  

Objective:  
Determine the user requirements of the system to be developed  

Methods to collect information of user’s requirements:  
Aspects: economic, organizational, technical in a feasibility study  

_**Questionnaire and survey**_  
Definition:  
A set of questions in written format so as to get information from individuals  
Use:  
Collect some general data which the information required is large  

_**Interview**_  
Definition:  
Asking questions on one-to-one basis on what the user expects the system will do  
Use:  
Elicit users’ requirements because it is simple and direct  

_**Observation**_  
Definition:  
Watching processes being done by users, the analyst see the reality of the operation  
Use:  
Let analysts gain a first-hand experience of how users interact with the current system  

_**Document review**_  
Use:  
Examine the documents used  

A set of complete description of the requirements of the system to be developed  

#### Feasibility study  

Objective:  
Determine whether the purpose of developing a system is justified  
Use:  
Propose alternative solutions and make a recommendation  

* **_Technical feasibility_**  

Whether the solution can be supported by existing technology  
Candidate system can provide appropriate responses to what extent it can support the technical enhancement

* **_Economic feasibility_**  

A cost-benefit analysis => measures the financial risks associated with the project  
Development costs - developing (one time cost)  
Operation costs - maintaining (recurring cost)  

* **_Organizational feasibility_** (Operational feasibility)   

Whether the solution can be integrated into the ongoing business of the organization.  
Whether the system could work effectively once it is developed and implemented.  

* **_Behavioural feasibility_**  

Evaluate and estimate the user attitude towards the development of the system.  

* **_Schedule feasibility_**  

Whether the development can be completed within given time constraint.

Formulate and evaluate alternative proposals  
After feasibility study, several possible solutions may be proposed  

Write requirement specifications:  

* Define the functions of the system  
* Define the Performance Specification  
* Define the User Interface  
* More…  

### Systems Design  

Suitable data structures and algorithms are used for delivering functions for the program  

_**User Interface**_  
It defines how a system interacts with its users => affect acceptance and usability  

Six principles:  

* Layout of screen, form and report  
* Content awareness  
* Aesthetics  
* User experience  
* Consistency  
* Minimize user effort  

Type of user interface:  

* __Command-driven interface (CLI)__
    - Interact via text terminal  
    - User has to remember all commands => difficult to use  
* __Menu-driven interface__  
    - Interact through a list of choices  
    - No need to remember commands => more user friendly than command  
* __Graphical user interface (GUI)__  
    - Interact through graphical icons  
    - Very common  
    - A pointing device can be used  
    - Characterized by WIMP (Windows, Icons, Menus, Pointing device)  

_**Modeling tools**_  
Data and process of a system can be modeled with data and process modeling tools  

Reason to use modeling tools:  
To avoid ambiguity that exists in natural languages  

* __Entity relationship diagram__ (ERD)  
* __Data flow diagram__ (DFD)  

Process model with DFD  
To describe how:  

* The processes or activities are performed  
* Data moves among them so as to accomplish the system goal  

4 symbols:  

* Process  
* Data flows  
* Data stores  
* External entities  

DFD describe the system at different levels of details => support different type of users  
(E.g. a librarian would need to know the key functions of a library information system, but not how the functions are delivered)  

__Context diagram__ is the highest level of a DFD, shows how the overall system work  
Each process in a DFD may be expanded into lower level DFD  
The first level of DFD below context diagram is called a level 0 diagram  

__Data dictionary__  
Definition: a set of metadata that describes the definitions and representations of data  

_**System flowchart and structure chart**_  

__Flowchart__:  
It graphically represents various programs, files, databases and manual processes.  
Symbols are labeled and connected.  

__Structure chart__:  
It describes the structural relationship and information exchanged by functions in a program.  

3 components:  

* Module  
* Connections (between modules)  
* Communications (of data)  

**_Project planning_**  

__Critical path method__ (CPM):  
To helps project managers to monitor project progress during the project period  
To helps project managers to identify which task is critical  
(if critical path delayed, the whole development will delay)  

Steps:  

1. List all task with  
    1. Earliest start date  
    2. Estimated length of time required  
    3. Any preceding tasks  
2. Represent the task with arrows and circles  

Major benefits: helps compute the project duration and monitor project progress  
Software tools: Microsoft project  

__Gantt chart__  
Definition: a type of bar chart that illustrates a project schedule  
Software tools: GanttProject  

### Systems Implementation  

Phases:  

* Program coding => realization and actualization of the abstract models  
* System testing => identify errors and inadequacies  

System testing:  

* Compare the actual results with the expected results  
* Should be performed in different development stages => cheaper to fix  

Type of testing:  

1. Unit testing => ensure the function of individual modules  
2. System testing => evaluate the entire system (usually done by system analyst)  
3. Acceptance testing => carried out by the users to ensure the requirements are met  
    1. Alpha testing, using made up test data  
    2. Beta testing, using real data  

**_Test Plan_**  
Definition: a series of tests to be carried out in a systematic way to test a system  
Content:  

* Test number  
* Requirement addressed  
* Test cases  
* Expected result  
* Actual result  

### Systems Conversion  

Types of strategies:  

* Direct cutover conversion  
    - Pros  
        - Simple and straightforward  
        - Cost the least  
    - Cons  
        - Difficult to switch back to the old system  
    - Errors in the new system can be fatal  

* Parallel conversion  
    - Pros  
        - Compare new and old to uncover flaws  
        - Old system serves as backup  
    - Cons  
        - Extra expenses  
        - Workload of user is doubled  

* Phased conversion  
    - Pros  
        - Errors can be fixed without long standstill  
        - Cost less than parallel, because users are not required to do twice  
    - Cons  
        - Take long time for new system to be fully installed  
        - Compatibility of new and old system maybe difficult to implement  

* Pilot conversion  
    - Pros  
        - Errors only in pilot site, limits harm to the entire organization  
        - Other sites can learn from the pilot site  
    - Cons  
        - Pilot site’s successful operation does not guarantee other sites’ operation  
        - A considerable amount of time to install in all sites  

### Systems maintenance  

Partly definition: on-going support  
Include: maintaining, upgrading, training  

* Fixing bugs (cannot fulfill user requirements)  
* System recovery after crash  
* System enhancement (perfect the system and additional features)  
* System integration (integrate multiple systems)  
* Underlying software or network change (new OS, DBMS, hardwares)  
* User assistance (online support, FAQs, staff support)  

**_User training_**  
Objective:  

* Help users to accomplish their tasks  
* Train on what the users need to do  

Training methods:  

* Classroom training  
* One-to-one coaching  
* Computer-based training (CBT)  

### Systems Documentation  

Objective: to help new personal to learn the system  
It is a on-going process throughout SDLC  

Type of documentation:  

* Program documentation  
    - System documentation, to help analysts and programmers to understand the whole system  
    - Technical documentation, to help programmers to learn the subsystems  
* User documentation, to help user, training, and online support  
    - User manual, to teach user to operate the system

**_Alternative Approaches in Systems Development_**  

__Drawbacks__ of Waterfall Model:  

* Clients only have vague idea => user requirement can’t be well identified before program coding  
* Can’t change user requirement midway => makes changes to preceding phases is difficult  
* Errors in the early phases cannot be detected until implemented  
* Long time from proposal to delivery of any usable system  

∴Water model is lack of flexibility  

Alternatives:  

* __Prototyping__  

A simplified version of the system is proposed to clients to collect early feedbacks (iteration) => fewer changes in later stages  
Drawbacks:  

    - Both analysts and clients focus only on user interface design, and too little on the producing of program code and functionality  
    - User may keep on providing minor feedbacks to add new requirement (scope creep)  
    - The constant changes may eventually lead to the system to become different from the original design, and make it look poor  

* __Rapid Application Development__ (RAD)  

It uses computer-aided software engineering (CASE) tools to assist  
Drawbacks:   

    - Same as prototyping  
    - Require highly skilled developers/designers  
    - Have to be able to be modularized  
