# MECA-482-Project
Furuta Pendulum 

Spring 2022, California State University of Chico

Andrew Davis- Crystal Farrand- Brandon Loeb- Nickolas Hofmann

### Table of Contents
- [1. Introduction](#1-Introduction)
- [2. Modeling](#2-Modeling)
- [3. Sensor Calibration](#3-Sensor_Calibration)
- [4. Controller Design and Simulations](#4-Controller_Design_and_Simulations)
- [5. Appendix](#5-Appendix)
- [6. References](#6-References)

## 1. Introduction
The Furuta Pendulum, a rotational inverted pendulum, was invented in 1992 at Tokyo Institute of Technology by Katsuhisa Furuta and his colleagues. Often used to demonstrate nonlinear control laws, the inverted pendulum consists of a driving arm which rotates in the horizontal plane and the pendulum attached to that arm, which is free to rotate in the vertical plane. The objective of this project is to design and implement a state-feedback control system that will balance the pendulum in the upright, vertical position. This requires deriving a mathematical model of the Furuta Pendulum and a controller for the system which can be inputted into MATLAB. Coppliasim will then be used to create a simulated version of the system that can be linked back to MATLAB. Together, MATLAB will act as the controller of the Coppeliasim simulation. 

##### Figure 1: Furuta Pendulum

## 2. Modeling
##### Figure 2: Furuta Pendulum Conventions
The diagram shown in Figure 2 above lists the conventions of the system. Based upon the variables listed, the angle 𝜃 lies between the rotary arm and the pendulum and the angle 𝛼 describes the inverted pendulum angle. The angle 𝛼 will be equal to zero when perfectly upright and balanced. Both angles are derived taking into account that a counterclockwise rotation will result in a positively increasing angle. A counterclockwise rotation occurs when the control voltage is positive. 

Matlab pic

## 3. Sensor Calibration 
This project does not include the physical implementation of the inverted pendulum and therefore does not need to be calibrated. Any physical system should be tested to ensure that the rotary arm angle and pendulum angle increases positivity when rotated counterclockwise as dictated by an applied positive voltage. These assumptions are based upon the model conventions declared above.

## 4. Controller Design and Simulations 

## 5. Appendix

## 6. References 
