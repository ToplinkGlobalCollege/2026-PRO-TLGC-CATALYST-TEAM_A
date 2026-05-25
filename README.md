Engineering materials
====

This repository contains engineering materials of a self-driven vehicle's model participating in the PRO Future Engineers competition in the season 2026

# Content
**docs**- Contains all documentation for the project, including robot architecture, programming flow, assembly instructions, improvement logs, and team information.

**hardware**- Contains EV3 hardware related files such as chassis designs, wiring layouts, and parts lists.

**media**- Contains visual assets such as robot photos, design diagrams, wiring schematics, and video recordings.

**software**-  Contains all source code for the EV3 robot. This includes the main control program developed using LEGO Mindstorms, which manages motor control and sensor input to perform tasks and navigate the environment.


> [!NOTE]
> This README.md doesn't contain all the information, some details are inside the folders

## Introduction
This document presents the technical specifications and design details of the TLGC Catalyst Future Engineer's Team A's autonomous vehicle robot for the 2026 Philippine Robotics Olympiad.

## TLGC Robotics Catalyst Team
Our team consists of two dedicated members who carefully manage the key aspects of our autonomous vehicle’s development. Representing Toplink Global College, the Future Engineers Team A is a passionate group committed to optimizing the essential electromechanical systems that drive our fully autonomous robot.


**Tymothy P. Dobla**

[![Facebook](https://img.shields.io/badge/Facebook-Follow-1877F2?style=flat&logo=facebook&logoColor=white)](https://www.facebook.com/iwwfyeiitahy)

**Zen Kobin N. Tevar**

[![Facebook](https://img.shields.io/badge/Facebook-Follow-1877F2?style=flat&logo=facebook&logoColor=white)](https://www.facebook.com/tevar.zenkobin)

> [!NOTE]
> The team information is at the docs folder
# Materials
Our autonomous self driving car was developed using the LEGO Mindstorms EV3 Education Set (45544) and LEGO Mindstorms Education EV3 Expansion Set (45544)

![45544-1-0-removebg-preview](https://github.com/user-attachments/assets/7b6e5ab7-0c0d-43d3-89e1-20ac8d9be258)
<img width="500" height="500" alt="Lego Mindstrom Expansion Set " src="https://github.com/user-attachments/assets/54831924-3041-4191-8ca0-946f1caf6f2f" />


> [!NOTE]
> The list of the materials used in our robot is inside the hardware folder

# Chassis

## Selection Of Wheel
<img width="4096" height="3072" alt="received_1900753783947376-Arc" src="https://github.com/user-attachments/assets/824e90f7-6fc8-43f1-bb90-490fa8866875" />

We selected the Wheel 39367 at the front and the Wheel 49295 at the rear to optimize our robot’s performance on a mat field. The front wheels are lightweight and have a low friction, narrow profile, which allows for quick, smooth turns with minimal resistance perfect for precise navigation on a smooth surface. Their design supports agile repositioning during autonomous routines where accuracy and responsiveness are critical. This configuration delivers an ideal balance of maneuverability at the front and powerful drive at the back, allowing the robot to move efficiently, accurately, and reliably on a mat based competition field

## Execution of Motors And Its Engineering Factor

### Motor Used For Steering
<img width="4096" height="3072" alt="received_1900753783947376-arc-motor" src="https://github.com/user-attachments/assets/1a8bc634-8115-4711-8c65-dea33ef9c912" />

The medium motor is small and fast, which makes it perfect for turning the front wheels quickly and smoothly. This helps the robot steer accurately when changing direction or making turns on the mat.

### Motor Used For Power
<img width="8160" height="6120" alt="Drive motor" src="https://github.com/user-attachments/assets/8c871a10-1e16-49fd-ab05-91d4b9df403f" />

The medium motor at the back gives the robot its main driving power. It provides strong and steady movement, allowing the robot to move with good speed and stability. This setup—steering in the front and power in the back—keeps the robot balanced and allows it to move smoothly, turn precisely, and stay in control on the mat field during the competition.

## Engineering Principle

Based on a simple engineering principle "Use the right tool for the right job". Steering doesn’t need a lot of power instead it needs to be quick and light. That’s why we chose the medium motor. It’s smaller, faster, and helps the robot turn smoothly without slowing it down. Driving the robot forward, on the other hand, needs strength and stability. That’s where the medium motor comes in. It’s more powerful and gives the robot the force it needs to move across the mat with steady speed and control. Putting it at the back also helps the robot stay balanced and keeps the rear wheels from slipping.

This setup follows the principle of separating movement and control we use a light motor for turning and a strong motor for moving. It makes the robot easier to steer, stronger when driving, and overall more reliable during the competition.

## Execution Of Steering
<img width="4096" height="3072" alt="received_1716336013050656-arc-steer" src="https://github.com/user-attachments/assets/772a3e71-6e5a-4e9e-b333-894487e28556" />

Our robot uses a front steering mechanism inspired by the rack and pinion system to control its direction. Instead of a full gear rack, we used a half gear piece connected to a beam. When the gear rotates, it pushes the beam side to side, which turns the front wheels left or right. This setup allows the robot to steer smoothly and accurately, making it easier to change direction on the mat. The system provides controlled and stable movement during turns, helping the robot navigate the field more consistently during competitions.

# Energy and Sensor Management
This section covers the power source of the self driving car and the sensors used to provide it with the necessary information to navigate various challenges. It explains the reasoning behind the selection of each sensor and how they are integrated into the car, along with details on power consumption. A wiring diagram is also included for reference.

## Energy Source
We’ve powered our self-driving car using the EV3 rechargeable battery, which provides a stable energy supply to ensure smooth and consistent operation. This battery serves as the main power source for our robot.

<img width="1335" height="1696" alt="Battery Source" src="https://github.com/user-attachments/assets/5939e7b1-b03f-4d41-bfef-d27653e3c9d5" />

### Ultrasonic Sensor
Our robot utilizes an ultrasonic sensor to determine its distance from the field wall. The sensor emits sound waves and measures the time it takes for the echo to return, calculating the exact distance based on that delay.

## Code & Control Used
<img width="1127" height="578" alt="62a79050e42d729d928b1756" src="https://github.com/user-attachments/assets/d2981cff-b953-4dc6-96d0-b0aa0891b07b" />

We used Python in Visual Studio Code to program our EV3 robot, managing motor control and sensor input to perform tasks and navigate its environment.

# Code Management
## Open challenge

<img width="1646" height="880" alt="image" src="https://github.com/user-attachments/assets/08d0403d-067c-4cea-a052-5c687eeebaed" />
