```
# EXPERIMENT--01-ALP-FOR-8086
Name :
Roll no 
Date of experiment :
```





## Aim:

## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output:
<img width="1694" height="964" alt="Screenshot 2025-08-22 153936" src="https://github.com/user-attachments/assets/079a6944-ccf3-4789-8d57-173ddaa4e8e1" />
## Subtraction   of 8 bit numbers  ALP :
```
 MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output:
<img width="1685" height="968" alt="Screenshot 2025-08-22 160749" src="https://github.com/user-attachments/assets/07d5a705-6ba7-490f-a45a-0563b1120649" />
## Multiplication alp:
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output:
<img width="1707" height="974" alt="Screenshot 2025-08-22 162133" src="https://github.com/user-attachments/assets/be481c3c-dd74-4b79-a513-fe4f5129d611" />
## Division alp:
```

MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output:
<img width="1749" height="983" alt="Screenshot 2025-08-22 162634" src="https://github.com/user-attachments/assets/ebd987a7-0eb1-4c62-9f4f-905cf66a289b" />
## LOGICAL OPERATOR:
## AND OPERATOR:
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT:
<img width="1698" height="981" alt="Screenshot 2025-08-29 153113" src="https://github.com/user-attachments/assets/9d9a752f-c139-4425-b1b8-73d726610b3e" />
## OR OPERATOR:
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT:
<img width="1849" height="974" alt="Screenshot 2025-08-29 153315" src="https://github.com/user-attachments/assets/db1ead30-3631-45ad-968f-56282b75455b" />
## NOR OPERATOR:
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT:
<img width="1700" height="970" alt="Screenshot 2025-08-29 153430" src="https://github.com/user-attachments/assets/c96b4e55-aa9a-40f6-9edf-00875a91922d" />
## NAND OPERATOR:
```

MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT:
<img width="1692" height="968" alt="Screenshot 2025-08-29 153524" src="https://github.com/user-attachments/assets/dad8a18b-13b4-43c4-892b-da46a26ff1b7" />
## NOT OPERATOR:
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```
## OUTPUT:
<img width="1727" height="974" alt="Screenshot 2025-08-29 154426" src="https://github.com/user-attachments/assets/29a39f03-225a-451e-a006-cb73274a6354" />
## XOR OPERATOR:
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT:
<img width="1673" height="967" alt="Screenshot 2025-08-29 154627" src="https://github.com/user-attachments/assets/dc21cef4-e817-4180-9ae4-6cd1b8dc4efa" />
## Result :
This program was created sucessfully

 








