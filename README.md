# MECA-482-Project
Furuta Pendulum 

Spring 2022, California State University of Chico

Andrew Davis- Crystal Farrand- Brandon Loeb- Nickolas Hofmann

### Table of Contents
- [1. Introduction](#1-Introduction)
- [2. Modeling](#2-Modeling)
- [3. Sensor Calibration](#3-Sensor_Calibration)
- [4. Controller Design and Simulations](#4-Controller_Design_and_Simulations)
- [4.1. Balance Control](#4.1-Balance_Control)
- [4.2. Swing-up Control](#4.2-Swing-up_Control)
- [5. Controller Implementation](#5-Controller_Implementation)
- [6. References](#6-References)
- [7. Appendix](#7-Appendix)

## 1. Introduction
The Furuta Pendulum, a rotational inverted pendulum, was invented in 1992 at Tokyo Institute of Technology by Katsuhisa Furuta and his colleagues. Often used to demonstrate nonlinear control laws, the inverted pendulum consists of a driving arm which rotates in the horizontal plane and the pendulum attached to that arm, which is free to rotate in the vertical plane. The objective of this project is to design and implement a state-feedback control system that will balance the pendulum in the upright, vertical position. This requires deriving a mathematical model of the Furuta Pendulum and a controller for the system which can be inputted into MATLAB. Coppliasim will then be used to create a simulated version of the system that can be linked back to MATLAB. Together, MATLAB will act as the controller of the Coppeliasim simulation. 

![Figure 1](https://user-images.githubusercontent.com/104535058/168446020-45609705-000b-463b-89ad-1030e034c548.PNG)

#### Figure 1: Furuta Pendulum

## 2. Modeling
![Figure 2](https://user-images.githubusercontent.com/104535058/168445992-2a1bd987-6306-4cb4-b53e-5913ebe65b74.PNG)
##### Figure 2: Furuta Pendulum Conventions
The diagram shown in Figure 2 above lists the conventions of the system. Based upon the variables listed, the angle 𝜃 lies between the rotary arm and the pendulum and the angle 𝛼 describes the inverted pendulum angle. The angle 𝛼 will be equal to zero when perfectly upright and balanced. Both angles are derived taking into account that a counterclockwise rotation will result in a positively increasing angle. A counterclockwise rotation occurs when the control voltage is positive. 

Matlab pic

## 3. Sensor Calibration 
This project does not include the physical implementation of the inverted pendulum and therefore does not need to be calibrated. Any physical system should be tested to ensure that the rotary arm angle and pendulum angle increases positivity when rotated counterclockwise as dictated by an applied positive voltage. These assumptions are based upon the model conventions declared above.

## 4. Controller Design and Simulations 
## 4.1. Balance Control
The conventions of the system listed above are not satisfactory to design the control system for the Furuta Pendulum. The needed information is listed below in Table 1. Table 1 describes the necessary specification pertaining to the control design and time-response requirements for the system. 
#### Table 1: Control Specifications

![Table 1](https://user-images.githubusercontent.com/104535058/168490437-d3af9fa8-7d05-424f-adea-0d6a8ef4ab33.png)

Complimentary to the specifications of Table 1 above, the pendulum deflection and control effort requirements are to be satisfied when the rotary arm is tracking a 20 degree angle square wave.

MATLAB code

## 4.2. Swing-up Control
The concept of the swing up control is reliant on a nonlinear, energy based control scheme. The swing up control is implemented to get the pendulum from a downward vertical position to the upward position that is needed to initiate the balance control. 

MATLAB code

## 5. Contoller Implementation
(Optional)

## 6. References 

## 7. Appendix
[Appendix.pdf](https://github.com/Cnfarrand/Spring-Meca-482-Project/files/8693757/Appendix.pdf)
