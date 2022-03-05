# Program-Control-with-Hand-Gestures

I developed a project, using the capabilities of Arduino. I decided upon motion-controlling a media player, where the user is able to control a program (in this case, VLC Media Player) with hand gestures.  
The technique I used to detect hand gestures is called leap motion, which is included in some laptops and desktop computers, or Leap Motion controllers. This technique consists mainly in using hand or finger gestures as an input much like a mouse or a keyboard. 
In this report I will explain in detail how that came into fruition between the user interaction, the hardware configuration and the code.  


There are 3 main components to this project:
2 ultrasonic sensors (HC-SR04),
Arduino Uno (Arduino UNO R3 ATmega328P),
A computer 

The programs that were used are:
 Arduino IDE,
 PyCharm 

The sensors were connected to the Arduino (The pin configuration is shown in Fig.4). The Arduino is connected to the computer which provides power to the module and also establishes communication through a serial port (USB). 
The sensors measure the distance by emitting ultrasonic waves and receiving the reflected wave back from the target (in our case the target is the hand), then measure the time between the emission and reception. 
We place 2 ultrasonic sensors on top of the laptop one on either side: these will measure the distance from the hand to the sensor with the help of Arduino. 
Afterwards the Arduino will determine which gesture was made by the user and match it to the action command. Following that, the commands from Arduino are sent to the computer through USB.  
This data will then be read by python which is running on the computer and based on the read data an action will be performed. 

