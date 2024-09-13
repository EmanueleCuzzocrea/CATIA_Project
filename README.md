# Virtual Prototyping Final Project

## Overview
This project involves the virtual prototyping of an auxiliary equipment system designed to assist RH Facility operators in handling mockups
of First Wall modules for a Nuclear Fusion Reactor. The complete project assignment can be find in the Project_Assignment.pdf file. The entire project was developed in **CATIA**, and a modular solution was proposed, in which each component is actually available on the market.
Specifically, the proposal includes using a **KUKA KR 340 R3330 manipulator** for the movement of modules, positioned above a scissor lift,
the **P-8036 Scissors Lift by Advance Lifts**, in order to reach properly also the modules on the top. To make the entire structure mobile, we propose to put the system on an omnidirectional cart, namely a **Morello Omni**.
Additionally, a walkway, a ladder, and a toolbox have been designed to allow the operator ergonomic access to the RH Facility and easy access to all modules.
To verify the correct functioning of the system, **FEM analyses** were conducted to simulate the behavior of the structure under maximum load. The individual elements were analyzed, as well as the complete structure. Subsequently, **kinematic simulations** were performed, demonstrating how the
proposed solution allows access to all modules while avoiding singularity configurations of the manipulator.
Finally, **ergonomic analyses** were carried out using the Jack software.


## Table of Contents
1. [Introduction and Requirements](#introduction-and-requirements)
2. [Modelling](#modelling)
3. [FEM Analysis (FEM)](#finite-element-analysis-fem)
4. [Kinematic Simulations](#kinematic-simulations)
5. [Ergonomics](#ergonomics)
6. [Conclusions](#conclusions)

## Introduction and Requirements

The main objective of this project is to design a virtual prototype of an auxiliary equipment system designed to assist RH Facility operators in handling mockups of First Wall modules for a Nuclear Fusion Reactor. The project must meet the following functional requirements:

- Allow operators to reach all modules ergonomically.
- Enable visual inspection of the modules and the divertor by operators.
- Ensure that operators have their toolbox within easy reach at all times.
- Ensure correct handling of the modules once disassembled by the operator.
- Provide an adequate number of degrees of freedom.
- Be capable of lifting more than 250 kg.
- Be operable and actuated ergonomically by the operators.
- Be designed to avoid causing harm to operators, the First Wall modules, or any other components.

### Project Objectives

- Satisfy all the stated requirements.
- Avoid interfering with or altering the RH Facility structure.
- Avoid introducing tracks inside or outside the RH Facility.
- Minimize costs by renting standard products without the need for damage or modification.

<p align="center">
  <img src="https://github.com/user-attachments/assets/c9735269-3060-4aa5-8beb-9f9447a68a47" alt="Pseudocode" width="500"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/507d115b-ec13-443e-bebb-169f8730479d" alt="Pseudocode" width="500"/>
</p>


## Modelling

The proposed system comprises three main components:

1. **Robot Manipulator:** A 6-degree-of-freedom robot capable of reaching all modules. Modelled on the KUKA KR 340 R3330, which can lift up to 340 kg, slightly more than required.

<p align="center">
  <img src="https://github.com/user-attachments/assets/73842f84-379e-4cbd-ba23-781f9c412d30" alt="Pseudocode" width="500"/>
</p>

Modelled parts:
<p align="center">
  <img src="https://github.com/user-attachments/assets/e90eb86e-2082-4d6e-8c9f-6cb6e8da1f04" alt="Pseudocode" width="500"/>
</p>


2. **Elevator:** Capable of lifting the robot and supporting its weight. Modelled on the Advance Lifts Model P-8036 Scissors Lift, which can handle up to 3628 kg with a platform size of 1219.2 x 1828.8 mm.

<p align="center">
  <img src="https://github.com/user-attachments/assets/b5374b72-876a-4472-9d8e-517f62b18f02" alt="Pseudocode" width="500"/>
</p>

Modelled parts:
<p align="center">
  <img src="https://github.com/user-attachments/assets/c9dc9e5c-2f5b-4d70-a614-9bc79eeb7b25" alt="Pseudocode" width="500"/>
</p>



3. **Cart on Wheels:** Supports the combined weight of the elevator and robot, modelled on the basis of the Morello Omni, which is omnidirectional and customizable with a maximum load capacity of 10,000 kg.

<p align="center">
  <img src="https://github.com/user-attachments/assets/db67a13d-5a4b-48df-a022-1ac73a42a946" alt="Pseudocode" width="500"/>
</p>

Modelled parts:
<p align="center">
  <img src="https://github.com/user-attachments/assets/785ed5f3-ce3b-4d30-9c55-55cea844d0d4" alt="Pseudocode" width="500"/>
</p>


### Modelling Approach

A bottom-up approach was used to model and assemble the components. Specific attention was given to:

- **Realistic modelling:** Every component of the system was modelled while considering all its degrees of freedom.

https://github.com/user-attachments/assets/69a11f03-2794-437f-baa0-9c7851dea66f


- **Anti-Tipping Measures:** Placement of two 1500 kg counterweights to prevent tipping, especially when the robot is fully extended.
<p align="center">
  <img src="https://github.com/user-attachments/assets/1759c648-b508-414e-bcd9-0caedefaae62" alt="Pseudocode" width="400"/>
</p>


- **End Effector:** Fitted with pneumatic suction cups tailored to handle the various shapes and sizes of the First Wall modules.
<p align="center">
  <img src="https://github.com/user-attachments/assets/bb6d0ec6-4b17-40f6-89b0-c7eab4e9b0f2" alt="Pseudocode" width="400"/>
</p>

### Robot-Elevator-Omni system
<p align="center">
  <img src="https://github.com/user-attachments/assets/afcf64d1-d276-49fb-8e53-f2ee411738e8" alt="Pseudocode" width="400"/>
</p>


### Walkway, ladder, and toolbox
<p align="center">
  <img src="https://github.com/user-attachments/assets/6e2a6261-029e-486f-9f98-1a09551a159c" alt="Pseudocode" width="400"/>
</p>


## FEM Analysis

FEM analyses were conducted to simulate the structural behavior of the system under maximum load conditions.
The individual elements were analyzed, as well as the complete structure. Key findings include:

- **Material:** Steel with a yield strength of 250 MPa and a safety factor of 1.5, resulting in an allowable stress of 167 MPa.
- **Von Mises Stress Analysis:** To ensure stresses remain within permissible limits.
- **Displacements:** Maximum displacements were observed at the robot's end effector and the upper part of the elevator, but were within acceptable limits.
<p align="center">
  <img src="https://github.com/user-attachments/assets/36df0155-fedf-403a-9281-00680a1f228d" alt="Pseudocode" width="400"/>
</p>


## Kinematic Simulations

The Robot-Elevator-Omni system's kinematic simulations demonstrated its ability to reach all modules, including some theoretically reachable from the opposite side of the RH Facility.
This confirmed the system's capability to address all requirements without critical issues.

### Reaching the Outboard First Wall modules

https://github.com/user-attachments/assets/82420123-4555-4154-9b7c-5b4642edca78


### Reaching the Outboard First Wall modules

https://github.com/user-attachments/assets/330d7cbb-c8ab-43d0-ab35-5cfcbeb00a12



## Ergonomics

Ergonomic analyses were performed using Jack software, considering a 50th percentile male (175 cm height, 80 kg weight).
Two critical positions were analyzed: reaching the highest and lowest First Wall modules.

- **High Module Assembly:** 80% of the population could perform the task with a maximum L4/L5 load of 2580 N.
- **Low Module Assembly:** 70% of the population could perform the task with a maximum L4/L5 load of 2419 N.

Both scenarios were well below the critical value of 3400 N, indicating ergonomic safety.

### Assembly of the highest module

https://github.com/user-attachments/assets/5153eb2f-c06c-4937-942b-21ac58786129

### Assembly of the lowest module

https://github.com/user-attachments/assets/63562921-bda9-480b-934b-824122af651d


## Conclusions

The proposed system meets all project requirements and supports ergonomic operation within the RH Facility.
Potential improvements include:

- Positioning the toolbox on a mobile support.
- Enhancing lateral stability of the cart.
- Increasing operator safety on the walkway.
- Optimizing the connections between the cart, elevator, and robot.
- Adjusting the height of the walkway.
- Refining the end effector dimensions.
- Implementing an emergency program.


Thank you!
