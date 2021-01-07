# Genesis G80(RG3), GV80(JX1)

## 1. Project Overview
- This project item is made of 3 parts: Panel controller, HVAC main controller, Rear controller
- 3 parts are connected by CAN protocol to communicate each other
- The panel controller is made of 3 functions: Screen Touch System, TFT LCD, Haptic
- I was in charge of the entire software development of the screen touch system

## 2. Development Environment
-  Real-Time based OS Software Platform
-  IDE: Visual Studio, Compiler(Green Hills)
-  RH850F1L 64-bit Microprocessor | mXT449T(Screen Touch IC)

## 3. Challenging issues / Research and Solution / Result
This section demonstrates what was challenging issues, how to research them, and how to solve them

### Challenge #1 - Defining a specification(function, verification) of the touch screen system
Since this project was the first new project in our branch, there was not any guidance for the touch screen system

### Research and Solution #1
*(Step 1)* Searched a lot of academic materials relevant to the function and verification of the touch screen system<br>
*(Step 2)* Sorted out necessary information according to our project requirements<br>
*(Step 3)* Detailed all the functional elements of the touch screen system with functional safety requirements considered<br>
*(Step 4)* Finalized the specification with engineers of the cooperative company<br>
*(Step 5)* Verified functions of the touch screen system in a test laboratory with a robot arm machine<br>

### Result #1
Stabilized the functional requirements of the screen touch system and the verification process. the following presents the contents of the specification of the touch screen system.<br>
<p align="center">
<img src="./Img/GV80_prj3.jpg"><br>
Fig.1) the functional specification of the touch screen system
<p>

### Challenge #2 - Automating time-consuming manual programming by creating a software tool
There were too many kinds of graphic images (more than 100) according to vehicle options and regions. Whenever a lot of graphic images are changed at customer's request, the touch coordinates were programmed manually at that time to match these graphic images with touch coordinates. It caused time-consuming programming and miss matched problem between the graphic images and the touch coordinates.

### Research and Solution #2
*(Step 1)* Formulated the algorithm that calculates the touch areas and the coordinates according to the graphic images<br>
*(Step 2)* Designed the function that links data structure used in software program with information of the touch area<br>
*(Step 3)* Created the verification algorithm that checks overlapped touch areas, wrong connected data structure, and software program errors<br>
*(Step 4)* Programmed all the functions and algorithms by utilizing VBA programming, automating software code generation<br>

### Result #2
Stabilized the functional requirements of the screen touch system and the verification process. the following presents the contents of the specification of the touch screen system.<br>
<p align="center">
<img src="./Img/GV80_prj1.jpg"><br>
<img src="./Img/GV80_prj2.jpg"><br>
Fig.2) the software tool that generates and verified software program automatically
<p>
