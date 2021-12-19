# Rushi-315.Arduino-IDE-programs
Rushi-315.Arduino IDE programs  with ultrasonic sensor
ARDUINO
ARDUINO BOARD IMAGE

Arduino is an open-source hardware and software company that designs and manufactures single-board microcontrollers and microcontroller kits. Arduino features a series of microcontroller boards for various applications. The Arduino Uno microcontroller board based on the Microchip ATmega328P due to its simple design, universal compatibility and less cost has attracted people from various walks of life. Adding to it, the programming software environment i.e. The Arduino integrated development environment (IDE) is very simple to understand and use. Thus, Arduino UNO proves to be a good tool to get your hands dirty and gain valuable experience in building small projects for beginner level IoT enthusiasts. Also, it finds its place in the basic inventory of some highly sophisticated IoT projects.
More info at: https://www.arduino.cc/

ULTRASONIC SENSOR

US IMAGE

An Ultrasonic sensor is a device that can measure distance by using sound waves. It measures distance by sending out an ultrasonic sound wave which then reflects back from an object placed in front of it.
The sensor then calculates the time difference between the sending and receiving of waves and converts it to distance.


I/O - INPUT/OUTPUT IN GENERAL
In computing, input/output is the communication between an information processing system, such as a computer, and the outside world, possibly a human or another information processing system. Inputs are the signals or data received by the system and outputs are the signals or data sent from it.


I/O IN ARDUINO
The Arduino UNO R3 board is equipped with sets of digital and analog input/output (I/O) pin. These features PWM, RXT, TXD, GPIO, I2C pin activities. There are in total 14 Digital pins and 6 Analogue pins on the Arduino UNO R3 board. The analogue pins can be alternatively used as digital pins if configured to do so.


COMPONENTS
The following are the components required to perform the application:
Arduino Uno R3 board
BreadBoard
Ultrasonic Sensor
LEDs - 6 units
220Ω resistors - 2 units
Connecting Wires

SPECIFICATIONS
After understanding the Arduino board, Ultrasonic Sensor and gathering required components, Now it's time to implement a circuit doing the following:
When the distance of an object from the US Sensor is greater than 15cms, the LEDs glow in a clockwise pattern.
Whereas, when the distance of an object from the US Sensor is less than 15cmsthe LEDs glow in an anticlockwise pattern.


CODE EXPLANATION
Void Setup
The void setup function runs once initialising all the required pins on the Arduino board.
LEDs are connected to digital pins 5,6,7,9,10,11 of the Arduino board. These LEDs are in an active low configuration i.e. when the input signal is low, LED is turned ON.
Ultrasonic sensor’s Echo and Trigger pins are connected to pins 12 and 13 of the Arduino respectively.


Void Loop
The void loop function runs the code repeatedly.
First, the Ultrasonic Sensor sends an Ultrasonic Wave which is reflected back from the object in front. Then the Arduino board calculates the time interval between sending and receiving of the wave and converts it into the distance which is then stored in distance variable.
 Now, based on the distance value, the if and else condition statement is executed. So, if ‘distance>=15.00’ condition is true, the if block statements for glowing of LEDs in a clockwise pattern are executed.
And if the condition is false, the else block statements for glowing of LEDs in an anticlockwise pattern are executed.
The delay lines in the program help in the rhythmic control of glowing LEDs.


