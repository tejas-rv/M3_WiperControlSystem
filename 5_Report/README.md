# REPORT - WIPER CONTROL SYSTEM

## Abstract

* Wiper is an essential component that used to wipe raindrops or any water from the vehicle’s windscreen.
* The objectives of this project are to upgrade the older cars system by providing wiping system which is free from stopping in the middle of the screeen.
* The concept of this proposed wiper system is similar with other existing conventional wiper.
* Existing system manually used control stalk to activate wiper and the process of pulling up wiper is difficult to be handled. 
* The driver needs to switch on and off the control stalk and it will reduce the driver’s concentration during the driving.
* We HAve Used STM32F407VG Microcontroller which is ased on the ARM microprocessor. 

## Introduction - WIPER
A windscreen wiper is indispensable device used to wipe rain and dirt from a windscreen. 
Today, almost all automobile are equipped with windscreen wiper, often by legal requirement. 
Clear vision for the car driver is an important prerequisite for safety in road traffic. 
The wiper faithfully keeps the windscreen clear, moving back and forth across the windscreen countless times as they sweep the water away. 
Traditional windshield wipers are actuated by a single constant speed motor related to the wipers by a system of connecting rods, often called the wiper arm.

![image](https://github.com/tejas-rv/M3_WiperControlSystem/blob/main/1_Requirements/Wiper.png)

## Requirements - SWOT Analysis
| STRENGTHS | WEAKNESS | OPPORTUNITIES | THREATS 
|:---:|:---:|:---:|:---:|
| Low cost | NO SENSORS | Quick Solution | Semi-Manual Design, Involves Human Interface |


# Detail requirements
## High Level Requirements:

| ID | Description | Status (Implemented/Future)
|:---:|:---:|:---:|
|HLR-1| Wiper to and fro motion |Implemented|
|HLR-2| Automatic OFF in the Initial position |Implemented|
|HLR-3| Automatically turn ON/OFF the wiper when rain is there |Future|

##  Low level Requirements:

| ID | Description | Status (Implemented/Future)
|:---:|:---:|:---:|
|LLR-1| User shall be able to Turn ON/OFF the system |Implemented|
|LLR-2| User shall be able to control the speed |Implemented|

# 4W&#39;s and 1&#39;H

## Who:

* All the people who are having vehicle with windsheild.

## What:

* To remove the Water/Dust/Stain from windsheild.

## When:

* During Raining.

## Where:

* This can be used in all over the globe.

## How:

* users can use this code to ease their work and project.

## Software & Components
* Software - STM32CubeIDE
* Hardware - STM32F4DISCOVERY Discovery kit
* Hardware Description - The STM32F4DISCOVERY Discovery kit allows users to easily develop applications with the STM32F407VG high-performance microcontroller with the Arm® Cortex®-M4 32-bit core which runs upto 168MHz. It includes everything required either for beginners or experienced users to get started quickly
* Components - ST-LINK embedded debug tool, ST-MEMS digital accelerometer, digital microphone, audio DAC, LED, LCD Display and others.

![image](https://www.st.com/bin/ecommerce/api/image.PF252419.en.feature-description-include-personalized-no-cpn-medium.jpg)

## Flow Chart

![image](https://github.com/tejas-rv/M3_WiperControlSystem/blob/main/2_Design/FlowChart.png)

## Block Diagram

![image](https://github.com/tejas-rv/M3_WiperControlSystem/blob/main/2_Design/BlockDiagram.png)

## State Diagram
![image](https://github.com/tejas-rv/M3_WiperControlSystem/blob/main/2_Design/StateDiagram.png)


## HLTP - High Level Test Plan
* Requirement based Test case

| ID | Description | Status of Button | Expected output | Acctual Output
|:---:|:---:|:---:|:---:|:---:|
|HLR-1| At the time of Engine ON |Button Pressed Once| Engine On | Engine ON
|HLR-2| At the time of Engine OFF |Button Pressed Twice| Engine OFF | Engine OFF
|HLR-3| At the time of Wiper ON |Button Pressed Thrice | Wiper On | Wiper On - Direction Clk-Wise
|HLR-4| At the time of Wiper OFF |Button Pressed Four Times | Wiper Off | Wiper OFF - Direction Anti-Clk-Wise

##  LLTP - Low level Test Plan

| ID | Description | Status 
|:---:|:---:|:---:|
|LLR-1| Car ON |Passed|
|LLR-2| Car OFF |Passed|
