# Metamodeling - Embedded System (Vehicle Monitoring System)
By: Ghanim Alsuwaidi (厄尼姆)

Student ID: LS2321206

Target Model: Embedded System - Vehicle Monitoring System
#### FILES: labtwo, Testing, SNAPSHOT(plugin), testingMyPlugin
- labtwo: Main Meta modeling file
- Testing: Task two testing and creating childs.
- labtwo.updatesite-1.0.0-SNAPSHOT: Plugin
- testingMyPlugin: Plugin Testing

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


#### EMF Metamodeling:
|       Meta Model      |                     Testing Meta Model (Class Child Creation)                              |
| ----------------- | ------------------------------------------------------------------ |
| <img width="752" alt="metamodel" src="https://github.com/gj1997x/metamodeling/assets/148683770/49cccad0-aff5-42e5-84a2-48dd5c2a4860"> |<img width="635" alt="TestingModel-1" src="https://github.com/gj1997x/metamodeling/assets/148683770/d43d792f-c2a6-4a83-abb8-55d3c5fa6823">


The metamodel is a visual representation of how the various components of an embedded system for a vehicle monitoring system are organized and interact with each other. It is a high-level abstraction meant to facilitate understanding of the system's architecture and guide its implementation. There are alot of pusposes of building an EMF, such as that  EMF models are easily extensible. Furthermore, EMF also gives a form documentation that is very useful and can be integrated with different tools such as graphical editing, model transformation which allows for a more comprehensive development environment.The figure above represents the whole metal modeling of the system done by RM2PT. It can be clearly seen the classes with their type such as abstract class. Moreover, it can be seen that how are each class related with their references, multiplicity and their relationship name. Moreover, on the above right figure is the testing of the meta model by creating an instances of different classes and filling up their attributes with the approperaite data. Some of the instances are referenced depending on their design in the model with their relationships to other instances which are also specified.


#### Siruis - Graphical Modeling Language:
|       Graphical Design - Modeling      |                     Graphical Design Testing                              |
| ----------------- | ------------------------------------------------------------------ |
| <img width="547" alt="Defining Diagram (Task 2)" src="https://github.com/gj1997x/metamodeling/assets/148683770/15187c9d-efa8-460c-a0a2-136c464aa6f8"> |<img width="1280" alt="graphical diagram(Task 2)" src="https://github.com/gj1997x/metamodeling/assets/148683770/cfdb97a2-18e7-45b0-b1af-4d547026c356">

The tool that was used to create the graphical design modeling was Siruis. As been ilustrated from the first figure on the left, it shows how Siruis was used to create Nodes for each element, how references have been made which are the relation edges and the sections for each node. On the other hand, the figure on the right is the graphical modeler which shows the result of the graphical modeling that was desingned and displayes all the nodes created with their specified icons and their relations. Each relation is specified with different colours which makes it clear to identify which relations they are, what is the source node and the target node.

#### Xtext - Textual Modeling Language:

<img width="649" alt="Xtext (Task 3)" src="https://github.com/gj1997x/metamodeling/assets/148683770/2f95b06a-48e7-4942-9155-8c5ca23813db">

The main tool that was used to create the textual design modeling is Xtext. Xtext is very useful tool that does an automatic generation of the code which indicates the textual modeling of the model. The text editor also can be used as a way to represent the meta model that was made earlier and it does the same task as the graphical modeling.

#### Testing Plugin:
|       Graphical Modeling      |                     Textual modeling                              |
| ----------------- | ------------------------------------------------------------------ |
| <img width="952" alt="Graphical Modeling Testing(Task 4)" src="https://github.com/gj1997x/metamodeling/assets/148683770/bdde9cbf-ceb9-4c38-b43f-8ae59b6cc2d8">|<img width="1112" alt="Xtext - 4(Task 4)" src="https://github.com/gj1997x/metamodeling/assets/148683770/ed8d9e29-4a9e-4aa5-8af4-d623ac683634">

The plugin was created and tested for both languages. In the figure on the left shows the graphical modeling language such that nodes can be draged and inserted on the diagram and it will be added on the model. These elemnts can be filled with the required attributes and references. As illustrated in the figure, after filling the required attributes and providing the reference, these will reflect on the diagram such that arrows will be made and names will be changed to the specified ones. On the other hand is the textual editor were it does the same functions as graphical modeling but using codes to create the nodes which thieir references.
