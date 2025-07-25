# SMART_AGRI_ROVER
An Arduino Uno-based smart farming solution integrating moisture sensing, flame detection, servo-controlled irrigation, and automated water pumping to optimise crop watering. Includes Bluetooth-controlled vehicle movement via a mobile joystick to enhance farm automation and responsiveness.
## Demo Video
<a href="https://drive.google.com/file/d/1lS3v3zLEF5gMKj5gfEhwvtU1Y9bMLXQP/view?usp=sharing">Click Here to watch a demo video</a>
<img width="722" height="636" alt="image" src="https://github.com/user-attachments/assets/101e4f60-87ff-4f9c-8f05-156866ef370c" />

## Introduction
Agriculture plays a crucial role in sustaining human life, yet farmers 
face several challenges, such as monitoring soil moisture, detecting 
fire hazards, avoiding obstacles, and efficiently watering crops. 
Traditional solutions require separate machines for each function, 
making them costly, inefficient, and space-consuming. To address 
these issues, we have developed an agricultural rover that integrates 
multiple essential functions, including soil moisture detection, flame 
detection, obstacle detection, Bluetooth-controlled navigation, and 
automated water pumping into a single compact system. This rover 
not only reduces costs but also increases efficiency by automating 
multiple tasks through a single platform, making precision farming 
more accessible and effective.

## Components 
The agricultural rover consists of various components, each serving a 
general purpose and a specific function in the project: 

Soil Moisture Sensor – 
• General Function: Measures the moisture content in soil to 
determine water needs. 
• Project Application: Used to check soil moisture levels and 
decide whether irrigation is required. 
Relay Module – 
• General Function: Acts as a switch to control high-power devices 
using low-power signals. 
• Project Application: Operates the water pump, as the Arduino 
UNO cannot directly power high-current motors. 
 
IR Sensor – 
• General Function: Detects objects in its path based on infrared 
light reflection. 
• Project Application: Identifies obstacles in the rover's path and 
stops movement to prevent collisions. 
 
 Flame Sensor – 
• General Function: Detects fire or high heat using infrared 
radiation. 
• Project Application: Monitors the field for fire hazards and 
activates the water pump to extinguish flames. 
 
 Servo Motors (2 Units) – 
• General Function: Provides precise control over movement and 
positioning. 
• Project Application: One servo moves the soil moisture sensor up 
and down for accurate moisture detection. The other servo 
controls the water pump to spray water efficiently. 
 
 Motor Driver – 
• General Function: Controls the direction and speed of DC 
motors. 
• Project Application: Drives the rover's wheels, enabling 
movement across the field. 

LEDs – 
• General Function: Provides visual indicators for various system 
statuses. 
• Project Application: - Red LED: Turns on when the IR sensor detects an obstacle. - White LED: Acts as a night-vision flashlight for better visibility in 
low-light conditions. 

LCD Display – 
• General Function: Displays textual information to provide 
feedback on operations. 
• Project Application: Shows real-time updates on the rover’s 
current functions. 

Arduino UNO – 
• General Function: A microcontroller that processes inputs and 
controls outputs. 
• Project Application: Acts as the central unit managing sensor 
data, executing commands, and controlling various components. 

Bluetooth Module – 
• General Function: Enables wireless communication between 
devices. 
• Project Application: Allows remote control of the rover through 
a mobile app. 

Switch – 
• General Function: Manually turns a circuit on or off. 
• Project Application: Controls the water motor, allowing users to 
disable irrigation when not needed. 

9V Battery – 
• General Function: Provides power to small electronic devices. 
• Project Application: Powers the motor operations. 

12V Battery – 
• General Function: Supplies higher power for energy-intensive 
systems. 
• Project Application: Provides power to the entire system, 
ensuring smooth operation.

## Software Used
<li>Arduino Uno IDE</li>
<li>Bluetooth app: Arduino Bluetooth Controller </li>

## Working
The agricultural rover operates in the following systematic manner: 

Power Distribution: The 12V battery powers the motor driver, which 
steps down the voltage to 5V for the Arduino UNO, ensuring a stable 
power supply for all components. 

Movement Control: The rover’s wheels are controlled by the motor 
driver, which receives signals from the Arduino UNO via Bluetooth 
commands from a mobile app. 
 
 Soil Moisture Detection & Watering: 
• The servo motor lowers the soil moisture sensor to measure 
moisture levels. 
• If moisture is low, the water pump is activated to irrigate the 
field. 
• If moisture is sufficient, the sensor is retracted, and watering is 
stopped. 

Fire Detection & Suppression: 
• The flame sensor continuously monitors for fire hazards. 
• Upon detecting fire, the water pump is activated to spray water 
on the affected area. 

Obstacle Detection & Navigation: 
• The IR sensor detects obstacles in the rover’s path. 
• If an obstacle is detected, the rover stops immediately, 
preventing damage or collision. 
 
Bluetooth Remote Control: 
• The Bluetooth module enables wireless operation of the rover. 
• The user can control movement, activate/deactivate sensors, 
and execute functions via a mobile phone app. 

## Results
The agricultural rover successfully integrates multiple functionalities 
into a single, compact, and efficient system. The rover was tested in 
different conditions, and the results were as follows: 
• Soil Moisture Sensor accurately detected soil moisture levels, 
and the servo-controlled water pump irrigated dry areas as 
required. 
• Flame Sensor effectively detected fire hazards, triggering the 
water pump to extinguish flames. 
• IR Sensor prevented collisions by stopping the rover when 
obstacles were detected. 
• Bluetooth Module allowed smooth remote operation, enhancing 
user control and automation. 
• LCD Display provided real-time feedback on rover actions, 
ensuring transparency in function execution. 
• The rover functioned efficiently on a single power system, 
reducing the need for multiple separate devices.

## Conclusion 
The Smart Agro Rover successfully addresses the key challenges in 
farming, integrating soil moisture detection, fire detection, obstacle 
avoidance, and remote-controlled irrigation in a single device. This 
innovation improves efficiency, reduces operational costs, and 
enhances precision farming by automating critical processes. 
Compared to traditional separate machines for each function, this 
rover offers a cost-effective, compact, and smart solution for modern 
agriculture. Future enhancements could include solar power 
integration, AI-based decision-making, and GPS-based autonomous 
navigation for even greater efficiency and autonomy.

<img width="746" height="448" alt="image" src="https://github.com/user-attachments/assets/068b38c4-32eb-4682-b1a6-a16fbc2a643a" />
