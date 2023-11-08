# Metamodeling - Embedded System (Vehicle Monitoring System)
By: Ghanim alsuwaidi

Student ID: LS2321206

Target Model: Embedded System - Vehicle Monitoring System
#### The labtwo file contains the META MODEL. The Testing contains the instances and the design of my graphical meta model tool.

### VMS - Vehicle Monitoring System
The Vehicle Monitoring System (VMS) is a comprehensive solution designed to enhance vehicle safety, efficiency, and connectivity. It combines a range of embedded systems  to monitor vehicle performance, anticipate maintenance needs, ensure operational safety, and provide real-time data to drivers and remote monitoring centers.

### Key Components:

- Embedded System: Its the central processing unit that containes many key components such as the sensors, actuators, microcontrolls, motors, memory and batteries inorder for performing data processing and provide the expected actions.
- DeviceComponent: General abstract class for components with a specific attributes such as serial number and manufacturer. It acts as a super class for a specific device components.
- Microcontroller: It mainly processes data from sensors, controlls actuators and handle communication protocls.
- ArchitectureType: An enumeration that specifies the architecture of a microcontroller. Options include ARM, MIPS, AVR, x86, and SPARC.
- Actuators: It represents a device with attributes type, range, and input signal. It is controlled by a Microcontroller.
- Motor: It is also a device that has an attributes of power rating, speed, torque, and motor type. It is also controlled by a microcontroller.
- Sensors: These are sensing device that can be of different types which are defined by SensorType enumeration, like temperature, pressure, humidity, or accelerometer. It has attributes for range, sampling rate, and output signal, and operates with a microcontroller.
- SensorType: An enumeration that lists different types of sensors used in the system.
- Battery: Each component may have its own battery implemented with it or uses the main battery depending on its architecture and have an attributes of capacity, voltage, usage, charge cycles, battery name, and manufacturer. It is required by sensors to function.
- ConnectivityModule: Includes attributes such as communication protocol, bandwidth, and range. It can be included in the embedded system and can have memory integrated with it.
- Memory: it represents the memory of the system or the memory integrated within each component.
- 


#### EMF Metamodeling:

<img width="752" alt="metamodel" src="https://github.com/gj1997x/metamodeling/assets/148683770/49cccad0-aff5-42e5-84a2-48dd5c2a4860">

