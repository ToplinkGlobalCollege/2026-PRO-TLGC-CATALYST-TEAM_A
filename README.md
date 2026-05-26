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
Our team consists of two dedicated members who carefully manage the key aspects of our autonomous vehicle’s development. Representing Toplink Global College, the Future Engineers Team is a passionate group committed to optimizing the essential electromechanical systems that drive our fully autonomous robot.


**Tymothy P. Dobla**

[![Facebook](https://img.shields.io/badge/Facebook-Follow-1877F2?style=flat&logo=facebook&logoColor=white)](https://www.facebook.com/iwwfyeiitahy)

**Zen Kobin N. Tevar**

[![Facebook](https://img.shields.io/badge/Facebook-Follow-1877F2?style=flat&logo=facebook&logoColor=white)](https://www.facebook.com/tevar.zenkobin)

> [!NOTE]
> The team information is at the docs folder
# Materials
Our autonomous self-driving car was developed using the LEGO Mindstorms EV3 Education Set (45544), the LEGO Mindstorms Education EV3 Expansion Set (45560), the LEGO Education Spike Prime Set (45678), and the LEGO Education Spike Prime Expansion Set (45681).

![45544-1-0-removebg-preview](https://github.com/user-attachments/assets/7b6e5ab7-0c0d-43d3-89e1-20ac8d9be258)
<img width="500" height="500" alt="Lego Mindstrom Expansion Set " src="https://github.com/user-attachments/assets/54831924-3041-4191-8ca0-946f1caf6f2f" />
<img width="500" height="500" alt="Untitled_design__1_-removebg-preview (1)" src="https://github.com/user-attachments/assets/c603aab7-3eb5-4038-a25c-03d34adfa567" />
<img width="500" height="500" alt="Untitled_design__2_-removebg-preview" src="https://github.com/user-attachments/assets/42340646-9021-4c7b-b346-9a9699572622" />

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

Based on a simple engineering principle "Use the right tool for the right job". Steering doesn’t need a lot of power instead it needs to be quick and light. That’s why we chose the medium motor. It’s smaller, faster, and helps the robot turn smoothly without slowing it down. Driving the robot forward, on the other hand, needs speed and stability. That’s where the medium motor comes in. It’s more powerful and gives the robot the force it needs to move across the mat with steady speed and control. Putting it at the back also helps the robot stay balanced and keeps the rear wheels from slipping.

This setup follows the principle of separating movement and control we use a light motor for turning and also a light motor for moving. It makes the robot easier to steer, stronger when driving, and overall more reliable during the competition.

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

<img width="8160" height="6144" alt="ultrasonic" src="https://github.com/user-attachments/assets/766dca34-06e2-4009-b571-b803874b9e96" />

Originally, our robot relied on a color sensor that detected colors on the sides of the field to know when to turn. If a color was detected, the robot would turn in that direction accordingly. This method worked at the start, but it proved unreliable at times due to lighting changes or faded markings that made colors hard to detect. To make the system more stable, we switched to using a single ultrasonic sensor to guide the robot using the wall. This sensor measures how close the robot is to the side of the field. By maintaining a set distance from the wall, the robot stays perfectly on track. If it gets too close or too far, it gently turns to correct itself. This wall following method made the robot significantly more accurate, allowing it to turn smoothly without needing color lines at all.

## Gyro Sensor
<img width="8160" height="6144" alt="gyro" src="https://github.com/user-attachments/assets/75b3e327-287e-4772-9556-0578765c781f" />

A gyro sensor is attached to help the robot track how many full turns or laps it has completed. Because one full spin equals 360 degrees, the sensor continuously adds up the total angle as the robot rotates. We programmed the robot to stop once it hits 1100 degrees, which is slightly more than three full laps. This allows the robot to spin around smoothly and finish up close to its original starting point. As soon as it reaches that specific angle, it stops, ensuring it doesn’t over-rotate or drift off track.

## Pixy Camera
<img width="8160" height="6144" alt="Pixy" src="https://github.com/user-attachments/assets/afcb7dff-5fe8-4a13-adf0-142fe51e2d09" />

Our robot uses a Pixy2 camera to detect colored objects in front of it. In this setup, it looks for two specific colors, green and red, which tell the robot which way to go when it encounters an obstacle. If the Pixy2 sees a green object, the robot knows to turn left, and if it sees a red object, it turns right. This helps the robot make quick decisions during the run and choose the correct path based on the color it detects ahead.

## Color Sensor
<img width="8160" height="6144" alt="color sensor" src="https://github.com/user-attachments/assets/a08ec302-235e-4be0-96d3-afa64e41d1b5" />

A color sensor is attached, helping the robot count laps by tracking colored lines on the track. As it drives, the sensor looks down at the floor to detect when the surface color changes. We programmed the robot to recognize the blue and orange lines, adding a lap to its counter each time it crosses them. This allows the robot to keep an accurate tally of its progress automatically. Once it reaches the target number of laps, it stops right on cue, ensuring it finishes its run precisely where it's supposed to.

## Code & Control Used
<img width="1127" height="578" alt="62a79050e42d729d928b1756" src="https://github.com/user-attachments/assets/d2981cff-b953-4dc6-96d0-b0aa0891b07b" />

We used Python in Visual Studio Code to program our EV3 robot, managing motor control and sensor input to perform tasks and navigate its environment.

# Code Management
## Open challenge

<img width="1646" height="880" alt="image" src="https://github.com/user-attachments/assets/08d0403d-067c-4cea-a052-5c687eeebaed" />

## Obstacle challenge

# Engineering Factor
We wanted our LEGO EV3 robot to have vision so it could follow lines, detect colors, and respond to objects. To do this, we used a PixyCam2 smart camera equipped with specialized LEGO firmware.

Because the EV3 uses proprietary ports that aren't natively compatible with the PixyCam's standard interface, we built a custom cable by cutting one end off a regular LEGO sensor cable to expose and splice the internal wires. We then coded the robot in Python, which allowed the EV3 brick to communicate with the PixyCam2 seamlessly, treating it just like any other standard LEGO sensor.

<img width="420" height="594" alt="595108374-e59a5707-6b38-432d-afe1-8f324c9f6016" src="https://github.com/user-attachments/assets/2993db83-a94a-44c1-bcc8-29cafa5f192b" />

Next, we attached the those wires to jumper wires compatible with the PixyCam2's small pin port. Referencing the Pixy LEGO firmware documentation, we matched the corresponding power, ground, and data lines, enabling the EV3 to recognize the PixyCam2 as a standard LEGO color or ultrasonic sensor. To prevent short circuits, we insulated the connections using electrical tape or heat-shrink tubing. Because both systems operate on a shared 5V power level, we did not need additional voltage conversion or protective circuitry to make it safe

<img width="433" height="577" alt="595111388-99acb471-f484-4434-b546-ef1eebb13a45" src="https://github.com/user-attachments/assets/2b11fe1e-415c-4d78-99eb-525341a02dce" />

Once everything was connected, our Python script established immediate communication between the EV3 brick and the PixyCam2. The camera continuously streamed real-time data—such as object locations and color signatures—which our Python code processed to dynamically control the robot's motors and actions. With this software-driven integration, our robot was able to follow lines, detect specific color targets, and track moving objects, delivering the high-performance responsiveness of an advanced machine using just a smart camera and LEGO parts.

To physically support this setup, we mounted the PixyCam2 using the small, L-shaped metal bracket that comes with the camera. By fastening it through the built-in screw holes, we were able to lower the camera's point of view, allowing it to focus sharply on the area directly in front of the robot. We manually adjusted the tilt before tightening the screws to lock it into position; even though this mounting setup wasn't motorized, it kept the camera perfectly stable during operation without requiring any extra parts.

# Improvements

We upgraded the robot by switching from two medium motors down to just one medium motor for driving, which allowed for a more compact and streamlined design. We also reduced our sensor setup from two ultrasonic sensors to just one ultrasonic sensor, freeing up enough physical space to integrate both a color sensor and a gyro sensor for much better navigation.

Regarding the vision system, we moved the camera from the top of the robot to the front, positioning it right above the steering motor for a clearer view. Lastly, we changed our steering setup; while our first robot used small wheels for steering, we have now upgraded to slightly bigger steering wheels while keeping the larger rear wheels, giving the robot improved turning precision, better traction, and smoother overall movement on the mat.

#1




# Credits
We are deeply proud to represent our school, Toplink Global College Inc., which constantly supports our passion for innovation and robotics. We also want to extend our heartfelt thanks to our beloved coach, your patience, guidance, and continuous encouragement truly inspired us throughout this journey. Finally, we express our sincere appreciation to LEGO Mindstorms; the high-quality components and flexible design of the EV3 kit provided the hands-on experience that allowed us to explore, build, and bring this project to life.




