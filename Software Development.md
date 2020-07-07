# Software Development

## Programming Languages Generations
### Generation 
Name: X Generation Language = XGL (X is a number)  

### First Gen - Machine language  
Machine language = machine code  
Properties:  
- Binary  
- **Machine dependent**  

### Second Gen - Assembly language  
Instructions are called mnemonic  
Code example:  
```
ADD dest, src  
```
`ADD`: opcode  
`dest` and `src`: operand  

Properties:  
- Directly control CPU  

### Third Gen - High level programming language  
Examples:  
- C/C++  
- Pascal  
- BASIC  
- Ada  
- Fortran  

Properties (Advantage):  
- Closer to human language and more like English  
- Machine independency  

Properties (Disadvantage):  
- Loss of direct control of CPU and memory address => less efficient  

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
Examples:  
- C  
- BASIC  
- Pascal  

### Declarative  
Focus on ‘what’ the goal is

### Logic Programming Language:  
Commonly used in AI  
Most well-known: Prolog (Programming in Logic)  
2 type of clause: facts and rules  

### Query Programming Language:  
Commonly used in database management system (DBMS)  
Most well-known: Structured Query Language (SQL/SEQUEL)  
Examples:  
- Oracle  
- Microsoft Access  

### Object-oriented Programming(OOP)  
Examples:  
- C++  
- Java  
- Python  
- JavaScript  

#### Objects 
Consist of multiple type of data that define properties of an object  
Consist of functions (methods) that define the behaviour of an object

#### Class
A template for object, so that multiple objects of the same properties (attributes) and functions (behaviours) can be created and stored  

#### Encapsulation:  
Advantage: access control (setter/getter)  
Explain:  
- Public variable (accessable from outside the class)
- Private variable (only accessable from inside the class)

#### Inheritance:  
Advantage: reusability  
Explain:  
- Inheritance/extend (functions or variables can be inherited to other classes)  

#### Polymorphism:  
Advantage: reusability  
Explain:  
Same name under different classes/objects are different  

### Criteria of Selecting a Language for a Specific Program
- Platform to be used
- Nature and size of the problem
- Program execution efficiency and hardware control
- Portability
- Program development time

_Revision with examples is better!_  
_Use the following **besttest** examples from the almighty Comp Soc!_  
_https://github.com/spc-comp-soc/spc-cs-db_

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
- Has its users  
- Has its purpose and some functions to offer  
- Has a boundary and well defined scope  
- May be composed of some sub-systems, their purpose are also clearly defined  
- Subsystems within the same information system interact  

### Developing a New System  
3 solutions:  
- Software package  
- In-house development  
- Outsourcing  

Factors on deciding:  
- Suitable package exists or not  
- Has suitable staff to develop or not  
- Cost-effective to develop in-house or not  
- Has reliable and experienced developers to take up outsourced project or not  
- Has suitable staff to administer the software or not  
- Project budget  
- More...  

### System Development Life Cycle (SDLC)  
Definition of SDLC:  
Conceptual model for development of an information system  
E.g. waterfall model, rapid application development (RAD)  

### The Waterfall Model  
Characteristics:  
- Sequential and linear  
- Phases with well-defined beginning and end points  
- Distinctive goals and end with deliverables  
- No turning back to a previous phase  

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
- Off-the-shelf softwares package => software packages
- In-house team => in-house development
- Hire a service provider => outsourcing

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

- **_Technical feasibility_**  
Whether the solution can be supported by existing technology  
Candidate system can provide appropriate responses to what extent it can support the technical enhancement

- **_Economic feasibility_**  
A cost-benefit analysis => measures the financial risks associated with the project  
Development costs - developing (one time cost)  
Operation costs - maintaining (recurring cost)  

- **_Organizational feasibility_** (Operational feasibility)   
Whether the solution can be integrated into the ongoing business of the organization.  
Whether the system could work effectively once it is developed and implemented.  

- **_Behavioural feasibility_**  
Evaluate and estimate the user attitude towards the development of the system.  


- **_Schedule feasibility_**  
Whether the development can be completed within given time contraint.

Formulate and evaluate alternative proposals  
After feasibility study, several possible solutions may be proposed  

Write requirement specifications:  
- Define the functions of the system  
- Define the Performance Specification  
- Define the User Interface  
- More…  

### Systems Design  
Suitable data structures and algorithms are used for delivering functions for the program  

_**User Interface**_  
It defines how a system interacts with its users => affect acceptance and usability  

Six principles:  
- Layout of screen, form and report  
- Content awareness  
- Aesthetics  
- User experience  
- Consistency  
- Minimize user effort  

Type of user interface:  
- _Command-driven interface (CLI)_
    - Interact via text terminal  
    - User has to remember all commands => difficult to use  
- _Menu-driven interface_  
    - Interact through a list of choices  
    - No need to remember commands => more user friendly than command  
- _Graphical user interface (GUI)_  
    - Interact through graphical icons  
    - Very common  
    - A pointing device can be used  
    - Characterized by WIMP (Windows, Icons, Menus, Pointing device)  

_**Modeling tools**_  
Data and process of a system can be modeled with data and process modeling tools  

Reason to use modeling tools:  
To avoid ambiguity that exists in natural languages  

- _Entity relationship diagram_ (ERD)  
- _Data flow diagram_ (DFD)  

Process model with DFD  
To describe how:  
- The processes or activities are performed  
- Data moves among them so as to accomplish the system goal  

4 symbols:  
- Process  
- Data flows  
- Data stores  
- External entities  

DFD describe the system at different levels of details => support different type of users  
(E.g. a librarian would need to know the key functions of a library information system, but not how the functions are delivered)  

_Context diagram_ is the highest level of a DFD, shows how the overall system work  
Each process in a DFD may be expanded into lower level DFD  
The first level of DFD below context diagram is called a level 0 diagram  

_Data dictionary_  
Definition: a set of metadata that describes the definitions and representations of data  

_**System flowchart and structure chart**_  

_Flowchart_:  
It graphically represents various programs, files, databases and manual processes.  
Symbols are labeled and connected.  

_Structure chart_:  
It describes the structural relationship and information exchanged by functions in a program.  

3 components:  
- Module  
- Connections (between modules)  
- Communications (of data)  


**_Project planning_**  

_Critical path method_ (CPM):  
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

_Gantt chart_  
Definition: a type of bar chart that illustrates a project schedule  
Software tools: GanttProject  

### Systems Implementation  
Phases:  
- Program coding => realization and actualization of the abstract models  
- System testing => identify errors and inadequacies  

System testing:  
- Compare the actual results with the expected results  
- Should be performed in different development stages => cheaper to fix  

Type of testing:  
1. Unit testing => ensure the function of individual modules  
2. System testing => evaluate the entire system (usually done by system analyst)  
3. Acceptance testing => carried out by the users to ensure the requirements are met  
    1. Alpha testing, using made up test data  
    2. Beta testing, using real data  

**_Test Plan_**  
Definition: a series of tests to be carried out in a systematic way to test a system  
Content:  
- Test number  
- Requirement addressed  
- Test cases  
- Expected result  
- Actual result  

### Systems Conversion  

Types of strategies:  
- Direct cutover conversion  
    - Pros  
        - Simple and straightforward  
        - Cost the least  
    - Cons  
        - Difficult to switch back to the old system  
    - Errors in the new system can be fatal  

- Parallel conversion  
    - Pros  
        - Compare new and old to uncover flaws  
        - Old system serves as backup  
    - Cons  
        - Extra expenses  
        - Workload of user is doubled  

- Phased conversion  
    - Pros  
        - Errors can be fixed without long standstill  
        - Cost less than parallel, because users are not required to do twice  
    - Cons  
        - Take long time for new system to be fully installed  
        - Compatibility of new and old system maybe difficult to implement  

- Pilot conversion  
    - Pros  
        - Errors only in pilot site, limits harm to the entire organization  
        - Other sites can learn from the pilot site  
    - Cons  
        - Pilot site’s successful operation does not guarantee other sites’ operation  
        - A considerable amount of time to install in all sites  

### Systems maintenance  
Partly definition: on-going support  
Include: maintaining, upgrading, training  

- Fixing bugs (cannot fulfill user requirements)  
- System recovery after crash  
- System enhancement (perfect the system and additional features)  
- System integration (integrate multiple systems)  
- Underlying software or network change (new OS, DBMS, hardwares)  
- User assistance (online support, FAQs, staff support)  

**_User training_**  
Objective:  
- Help users to accomplish their tasks  
- Train on what the users need to do  

Training methods:  
- Classroom training  
- One-to-one coaching  
- Computer-based training (CBT)  

### Systems Documentation  
Objective: to help new personal to learn the system  
It is a on-going process throughout SDLC  

Type of documentation:  
- System documentation, to help analysts and programmers to understand the whole system  
- Technical documentation, to help programmers to learn the subsystems  
- User documentation, to help user, training, and online support  

**_Alternative Approaches in Systems Development_**  

Drawbacks of Waterfall Model:  
- Clients only have vague idea => user requirement can’t be well identified before program coding  
- Can’t change user requirement midway => makes changes to preceding phases is difficult  
- Errors in the early phases cannot be detected until implemented  
- Long time from proposal to delivery of any usable system  

∴Water model is lack of flexibility  

Alternatives:  
- _Prototyping_  
A simplified version of the system is proposed to clients to collect early feedbacks (iteration) => fewer changes in later stages  
Drawbacks:  
    - Both analysts and clients focus only on user interface design, and too little on the producing of program code and functionality  
    - User may keep on providing minor feedbacks to add new requirement (scope creep)  
    - The constant changes may eventually lead to the system to become different from the original design, and make it look poor  

- _Rapid Application Development_ (RAD)  
It uses computer-aided software engineering (CASE) tools to assist  
Drawbacks:   
    - Same as prototyping  
    - Require highly skilled developers/designers  
    - Have to be able to be modularized  

## The Generation of Executable Files
High level languages are compiled into machine code for the computer to execute.  
Computer have a series of action to compile a program developed in programming language such as C/C++, Pascal, Java, etc.  

### Program Code Generation
_italic => (arrow)_: run-time process  
**bold => (arrow)**: compile-time process  

Program development  
**=>** Source code (.c)  
**=>** Compile (stop if compile-time error occurs)  
**=>** Object code  
**=>** Linker (links program libraries & shared libraries)  
**=>** Executable code (.exe) (in hard disks)  
_=>_ Loader (operating system) (loads dynamical-linked libraries)  
_=>_ Executable code (in main memory)  
_=>_ CPU (return if run-time error occurs)  
_=>_ Program result