# Virtual Prototyping Final Project

## Overview
This project involves the virtual prototyping of an auxiliary equipment system designed to assist RH Facility operators in handling mockups
of First Wall modules. The entire project was developed in **CATIA**, and a modular solution was proposed, in which each component is actually available on the market.
Specifically, the proposal includes using a **KUKA KR 340 R3330 manipulator** for the movement of modules, positioned above a scissor lift,
the **P-8036 Scissors Lift by Advance Lifts**, in order to reach properly also the modules on the top. To make the entire structure mobile, we propose to put the system on an omnidirectional cart, namely a **Morello Omni**.
Additionally, a walkway, a ladder, and a toolbox have been designed to allow the operator ergonomic access to the RH Facility and easy access to all modules.
To verify the correct functioning of the system, **FEM analyses** were conducted to simulate the behavior of the structure under maximum load. Initially,
individual elements were analyzed, followed by the complete structure. Subsequently, **kinematic simulations** were performed, demonstrating how the
proposed solution allows access to all modules while avoiding singularity configurations of the manipulator.
Finally, **ergonomic analyses** were carried out using the Jack software.


## Table of Contents
1. [Introduction and Requirements](#introduction-and-requirements)
2. [Modeling](#modeling)
3. [Finite Element Analysis (FEM)](#finite-element-analysis-fem)
4. [Kinematic Simulations](#kinematic-simulations)
5. [Ergonomics](#ergonomics)
6. [Conclusions](#conclusions)

## Introduction and Requirements

The main objective of this project is to design a virtual prototype of an auxiliary equipment system that meets the following functional requirements:

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

## Modeling

The proposed system comprises three main components:

1. **Robot Manipulator:** A 6-degree-of-freedom robot capable of reaching all modules. Modeled on the KUKA KR 340 R3330 is proposed, which can lift up to 340 kg, slightly more than required.
  
2. **Elevator:** Capable of lifting the robot and supporting its weight. Modeled on the Advance Lifts Model P-8036 Scissors Lift, which can handle up to 3628 kg with a platform size of 1219.2 x 1828.8 mm.

3. **Cart on Wheels:** Supports the combined weight of the elevator and robot, modeled on the basis of the Morello Omni, which is omnidirectional and customizable with a maximum load capacity of 10,000 kg.

### Modeling Approach

A bottom-up approach was used to model and assemble the components. Specific attention was given to:

- **Anti-Tipping Measures:** Placement of two 1500 kg counterweights to prevent tipping, especially when the robot is fully extended.
- **End Effector:** Fitted with pneumatic suction cups tailored to handle the various shapes and sizes of the First Wall modules.

## Finite Element Analysis (FEM)

FEM analyses were conducted to simulate the structural behavior of the system under maximum load conditions. Key findings include:

- **Material:** Steel with a yield strength of 250 MPa and a safety factor of 1.5, resulting in an allowable stress of 167 MPa.
- **Von Mises Stress Analysis:** Conducted for the robot, elevator, and cart to ensure stresses remain within permissible limits.
- **Displacements:** Maximum displacements were observed at the robot's end effector and the upper part of the elevator, but were within acceptable limits.

## Kinematic Simulations

The Robot-Elevator-Omni system's kinematic simulations demonstrated its ability to reach all modules, including those theoretically reachable from the opposite side of the RH Facility.
This confirmed the system's capability to address all proximity requirements without critical issues.

## Ergonomics

Ergonomic analyses were performed using Jack software, considering a 50th percentile male (175 cm height, 80 kg weight).
Two critical positions were analyzed: reaching the highest and lowest First Wall modules.

- **High Module Assembly:** 80% of the population could perform the task with a maximum L4/L5 load of 2580 N.
- **Low Module Assembly:** 70% of the population could perform the task with a maximum L4/L5 load of 2419 N.

Both scenarios were well below the critical value of 3400 N, indicating ergonomic safety.

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
