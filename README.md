# Fundamentals of Robotics and Robotic Automation

## 🤖 Simulation Preview
<img src="robotsim.png" alt="MATLAB Robot Manipulator Simulation" width="500" height="400"/>

## 📌 Project Portfolio Overview
In this repository, I showcase the engineering systems, mathematical models, and simulations I developed during the **Monash University Robotics Unit**. 

My work focused on the end-to-end design, kinematic modelling, dynamic simulation, and trajectory planning of serial robotic manipulators used in modern manufacturing and automation environments. 

***⚠️ Academic Integrity Notice:** In strict compliance with university academic integrity policies, my source code, custom Simulink models, and raw assignment files are withheld from public distribution. This README serves as a portfolio documenting the advanced engineering methodologies, algorithmic architectures, and core competencies I mastered throughout the project.*

## 🛠️ Core Engineering Capabilities 
* **Kinematics & Spatial Geometry:** Spatial descriptions and transformations, Denavit-Hartenberg (DH) parameters, forward kinematics (FK), and geometric/analytical inverse kinematics (IK) solver design.
* **Differential Kinematics:** Analytical and geometric Jacobian formulation, singularity analysis, and differential relationship mapping.
* **Rigid-Body Dynamics:** Formulation of equations of motion using both the energy-based **Lagrangian formula** and the recursive **Newton-Euler equations**.
* **Advanced Control Systems:** Synthesis of linear position controllers and high-performance **nonlinear motion controllers** (e.g., Computed Torque Control) paired with robust **force controllers** for interactive environments.
* **Trajectory & Task Planning:** Path planning algorithms, obstacle avoidance, joint-space vs. Cartesian-space interpolation, and automated task scheduling.
* **Industrial Automation:** End-effector configuration, workspace envelope appraisal, computational geometry for design and manufacture, and an introduction to mobile autonomous systems.

## 🎯 System Learning Outcomes Achieved
1. **Analyse Problems of Direct and Inverse Kinematics:** I formulated analytical and numerical algorithms to accurately resolve position and orientation state vectors for multi-DoF serial links.
2. **Generate Robotic Dynamics Models:** I established high-fidelity dynamic models utilising **Lagrangian and Newton-Euler paradigms** to predict joint torques and inertial forces under varying payloads.
3. **Design Linear and Nonlinear Controllers:** I architected closed-loop control strategies ensuring precise tracking, disturbance rejection, and optimal interaction force management.
4. **Design Robotic Tasks:** I synthesised complex, collision-free paths using advanced computational geometry to program automated manufacturing sequences.
5. **Appraise Serial Manipulator Performance:** I conducted comprehensive workspace optimisation and dynamic performance metrics evaluations to assess structural design efficiency.

## ⚙️ Technical Environment Covered
* **Primary Environment:** MATLAB (R2024a or later)
* **Core Toolboxes Utilised:** 
  * Robotics System Toolbox
  * Control System Toolbox
  * Symbolic Math Toolbox (for analytical Lagrangian derivations)
  * Simulink (for closed-loop control system evaluation)

## 📐 Algorithmic Architecture
The dynamics engine I worked with calculates the localised joint torque vectors $\tau$ explicitly via the manipulator dynamic equation:

$$\tau = M(q)\ddot{q} + C(q, \dot{q})\dot{q} + G(q) + J^T(q)F_e$$

Where:
* $M(q)$ represents the symmetric, positive-definite inertia matrix.
* $C(q, \dot{q})$ denotes the Coriolis and centripetal forces matrix.
* $G(q)$ is the gravitational vector.
* $J^T(q)F_e$ maps external end-effector wrench forces back into joint space via the transpose of the geometric **Jacobian**.

## 📜 Academic Attribution & Contact
This portfolio project was developed in alignment with the curriculum specified by the Department of Mechanical and Aerospace Engineering at **Monash University**. It serves as an architectural proof of concept for my skills in autonomous systems engineering, modern industrial robotics, and model-based design protocols. 

If you are a recruiter or fellow engineer and want to chat about the technical methodologies I used, please feel free to reach out to me!
