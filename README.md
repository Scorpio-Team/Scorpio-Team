### WRO 2022 FUTURE ENGINEERS

# Development Team

- Team Name : Nerdvana Scorpio
- Country : Romania
- Members : **Radu Timeea** ; **Damian Mihai** ; **Damian Alexandru**
- Coach : **Tutu Mihai**

# Youtube Video 



# Content

- **team** contains a photo of our team
- **Poze Robot** contains photos of the robot from various angles
- **video** contains a youtube link to a video of our vehicle running
- **schema** contains schematic diagrams of electronical components used in the building of our vehicle as well as how they connect
- **program** contains the source codes used for the robot  to function

# The Code 

We used two programing languages for the the vehicle. The source code written on the 
Raspberry Pi is written in Python whilst the source code written on the arduino is in c++.
The two boards communicate with eachother through serial. Both codes control diffrent parts of the robot but both come together to make the robot function.

- ## The Arduino Code
	
	1. The Ultrasonic Module contains the code used to control the ultrasonic sensors placed on the car, one placed on the left hand side of the car and one placed on the right hand side of the car.
	They are used to detect walls, which helps with the awerness of the robot. In turn, this can also be named The Wall Following module making the ultrasonic sensors one of the most essential parts of the robot.
	
	2. The Motor Module contains the code that controls the dc motor used for the movement of the robot as well as the servo motor 
	used for the steering of the vehicle. Both motors are connected to the arduino board, and using this module, we can control the speed of the car as well as the direction in which it is headed
	
- ## The Raspberry Pi Code

	- The Computer Vision Module uses the Raspberry Pi Camera Module V2 to input information into our Raspberry Pi and using that information and a little bit of code we can detect
	our colored blocks. Using this module, we can identify the color of the object, which we can comunicate to the arduino. With this information, the arduino
	can make the decision of going around the block on its right side or left side depending on the color.
	
# Electronics

In the making of our vehicle, we have used a total of 9 components that contribute to its function. All of them are described in great detail bellow, along with a schematic showing how they are connected to eachother

### 1. 1.5 V Rechargable Batteries.
	
Used to power all the components that are used in the build of our robot

### 2. Voltage and Amperage Regulator

Used to provide the correct voltage and amperage for the functionality of our components, 5V respectively 2A.

### 3. Raspberry Pi 3B

One of the most important components in our robot, the Raspberry Pi takes care of the color detection program that tells us which blocks are green and red, using code written in Python.
Along side the code we use the OpenCv library for object and color detection.

### 4. Raspberry Pi Camera Module V2 

This 8 megapixel native resolution capable of 4k static images as well as high quality video allows us to see what is infront of the car in great detail
and inputs that information into our raspberry pi where it will be procesed and used to detect the colored blocks neded for the correct functioning of the vehicle.

### 5. SparkFun RedBoard Qwiic

This board emulates an Arduino uno. It functions the same as the Arduino uno and it also has a lot of its features. The Sparkfun board has 20 Digital I/O Pins, 6 of which are PWM Outputs and 6 of which are Analog Inputs.
This board hosts the rest of the functionalities of the car, including *The Wall Following Module* and *The Motor Module* coded in C++, and it is vital to the functioning of the robot being the main componentused in its making.

### 6. The SparkFun Motor Driver - Dual TB6612FNG

This motor driver is used in the controlling of the DC Motor present in our vehicle. It is capable of controlling the motor in one of the 4 function modes: Clock Wise, Counter Clock Wise, Short-Brake and Stop as well as the speed of the motor
while managing the two motor outputs (A and B) seperately. 

### 7. Hobby Gearmotor

The Hobby Gearmotor has 140 RPM as well as a gearbox ration of 48:1 and it is used in the movement of the vehicle. The motor is placed on the backside of the car as seen in the photos attached.

### 8. Servo Motor 

The Servo is used in the steering of the car and is located in the front of the vehicle. This component is vital to our *Wall Following Module* as well as *The Computer Vision Module*.

### 9. HC-SR04 Ultrasonic Sensors

These sensors are used in *The Ultrasonic Module*. As seen in ***The Arduino Code*** section of this document, the sensors are placed on the left hand side and the right hand side of the robot, making any objects that are located to the sides of the car in between 2cm and 400 cm from the vehicle detectable.   
