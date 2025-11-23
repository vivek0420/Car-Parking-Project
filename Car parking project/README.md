🚗 Smart Car Parking System

Smart Car Parking System using Arduino Uno

📘 Abstract

The Smart Car Parking System aims to provide a smooth, confusion-free, and efficient parking experience. This project helps drivers park their vehicles with minimal time waste by showing real-time information about available parking spaces.

The system uses an Arduino Uno as the microcontroller, interfaced with ultrasonic sensors, servo motors, and an LCD display.

The LCD display shows available parking slots.

Ultrasonic sensors detect vehicle entry and exit.

Servo motors (optional) can be used as automated entry/exit barriers.

By continuously monitoring the presence of vehicles, the system ensures accurate parking-space updates.

📚 Theory

An automated parking system improves efficiency by eliminating the drawbacks of manual parking management. It counts the number of cars inside the parking area and determines whether any slots are available.

When a vehicle enters, the sensor detects it and increases the count.

When a vehicle exits, the count decreases.

The LCD display always shows the current number of cars and available slots.

If the parking lot is full, the system displays a “Parking Full” message.

The process relies on:

Arduino Uno to process sensor input

Ultrasonic sensors to detect vehicles

LCD to display the parking status

🔧 Hardware Components

Arduino UNO – Main microcontroller

Ultrasonic Sensors (HC-SR04) – Detect vehicle entry/exit

LCD Display (16x2) – Shows slot availability

Servo Motor (optional) – Gate control

Breadboard – Circuit prototyping

Power Supply – 5V/9V for Arduino and peripherals

Connecting Wires – Jumper wires for connections

📝 Features

Automatic vehicle detection

Real-time parking slot monitoring

Entry/exit counting

LCD screen displaying car count and slot availability

“Parking Full” alert

Simple, low-cost hardware setup

📂 Project Structure (Example)
/Smart-Car-Parking-System
│── /images
│── /code
│   └── SmartParking.ino
│── README.md

🚀 How It Works

Ultrasonic sensors detect movement of cars at the entrance and exit.

Arduino processes the distance readings and identifies if a car is entering or leaving.

The count of cars is updated accordingly.

The LCD display shows the updated parking information.

If maximum capacity is reached, the system displays “Parking Full.”
**Block Diagram**

![Block_diagram](https://user-images.githubusercontent.com/33668152/70372115-24bb3180-1905-11ea-9360-015bb582dfaf.jpg)



**Flow Chart**

![flowchart](https://user-images.githubusercontent.com/33668152/70372157-a1e6a680-1905-11ea-96c9-1e4bbbee5439.jpg)



**System Testing**

We have tested the design system with a dummy car. There are usually two possibilities.
•	Entry : While entering, the car is noticed by the sonars. Firstly the outer sonar and then the inner sonar. The count increases and result is shown in display.
•	Exit : In this case, Firstly the inner sonar notices and then the inner sonar. The count decreases and result is shown in display.

**Prototype**

![prototype](https://user-images.githubusercontent.com/33668152/70372162-c2166580-1905-11ea-8eef-45d700f4556e.jpg)



**Experimental Results**

We have experimented the system to gather some statistical results. After the experience, we have found the inner sonar and outer sonar works perfectly. As the result shows, the system is almost 100% correct. The whole experiment was done couple of times by us. Dummy cars were used. The prototype was not always correct due to the limitations of the use of low quality sensors. But the performance was satisfactory enough.

**References**

https://www.engineersgarage.com/electronic-components/16x2-lcd-module-datasheet

https://store.arduino.cc/usa/arduino-uno-rev3

http://www.micropik.com/PDF/HCSR04.pdf


