# Introduction
Serial communication is a common method of transmitting data between a computer
and a peripheral device such as a programmable instrument or even another computer.
Serial communication transmits data one bit at a time, sequentially, over a single
communication line to a receiver. Serial is also a most popular communication protocol
that is used by many devices for instrumentation.[7] This method is used when data
transfer rates are very low or the data must be transferred over long distances and also 
where the cost of cable and synchronization difficulties, make parallel communication
impractical. Serial communication is popular because most computers have one or more
serial ports, so no extra hardware is needed other than a cable to connect the instrument
to the computer or two computers together.
Introduction to ATmega328. ATmega328 is an Advanced Virtual RISC (AVR) microcontroller. It supports 8-bit data processing. ATmega-328 has 32KB internal flash memory.

# ATmega 328
ATmega328 has 1KB Electrically Erasable Programmable Read-Only Memory (EEPROM). This property shows if the electric supply supplied to the micro-controller is removed, even then it can store the data and can provide results after providing it with the electric supply. Moreover, ATmega-328 has 2KB Static Random Access Memory (SRAM). Other characteristics will be explained later. ATmega 328 has several different features which make it the most popular device in today’s market. These features consist of advanced RISC architecture, good performance, low power consumption, real timer counter having separate oscillator, 6 PWM pins, programmable Serial USART, programming lock for software security, throughput up to 20 MIPS etc. Further details about ATmega 328 will be given later in this section.

# Software used
### 1.SimullDE
### 2.Gcc compiler for AVR
### 3.Vs code

# ATmega238p to PC Serial Communication(RX/TX) using USART  

A collection of sample codes for communicating with Linux/Windows PC from an ATmega328p microcontroller using USART in asynchronous mode.

<img src = "https://www.xanthium.in/sites/default/files/site-images/atmega328p-usart-tutorial/atmega328p-pc-serial-communication-tutorial.jpg"/>

## Code

- Sourcecode written in **Embedded C**. 
- Compiled using **AVR-GCC** using **Make** utility.
- Code can be uploaded using AVRDUDE and any compatible programmer.

## Hardware setup

- Code tested on ATmega328p (32 pin TQFP).
- ATmega328p Clocked with a **11.0592MHz external crystal**.
- USB to Serial Converter used to connect ATmega328p with PC 
- PuTTY used to receive and Transmit data
- <img src = "https://www.xanthium.in/sites/default/files/site-images/atmega328p-usart-tutorial/atmega328p-serial-communication-pc.jpg"/>

## ATmega328p Clocking (Fuse Bits)
- External 11.0592MHz Crystal
- *avrdude -c usbasp -p m328p -U lfuse:w:0xFF:m*
- # Activity images
- ![image](https://user-images.githubusercontent.com/94265667/144376425-ec264d37-a523-4c5c-8ea3-c166bab5f53b.png)
- # Schematic diagram
- ![image](https://user-images.githubusercontent.com/94265667/144376824-8cade47b-dd63-4f2e-95a1-5c8761c58f2b.png)
- # Circuit diagram
![image](https://user-images.githubusercontent.com/94265667/144378622-6b0dce7b-0266-4461-99f5-7dd37a59e490.png)
# Implementation
## Introduction
This folder conatins all the coding files as well as the resources and testing files neede for proper execution of program
## Instructions to execute
1.Clone my repository
2.Go to 3_Implementation folder
3.Make sure your system meets all software and hardware requirements
4.Run "make run" command in terminal for main code execution
5.Run "make run_test" command in terminal for test code execution.
## Folder Structure
|Column 1 Header |Column 2 Header |
|--- |--- |
|Receiver |Main source code for system|
| | |
|Transmittet |Main source code for system|
| | |
|test |All source code and data for testing purposes|
| | |
# output images
![image](https://user-images.githubusercontent.com/94265667/144379551-fae97541-8184-464c-9d03-b8f4fdac3ddd.png)

![image](https://user-images.githubusercontent.com/94265667/144379670-2685b14b-1607-41c7-ad32-b7bfce3ca89f.png)

![image](https://user-images.githubusercontent.com/94265667/144379767-cbbc4dd7-e3d8-4886-9a9a-a00ba82fca81.png)






