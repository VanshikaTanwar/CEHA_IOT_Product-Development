# CEHA_IOT_Product-Development
CEHA = Cost-Efficient IOT Based Home Automation System .

Cost-Efficient IOT Based Home Automation System using VSDSquadron mini 
***CEHA-IOT, Powered by the VSDSquadron Mini***


TEAM VSD DIR-V-CEHA-IOT 


# Introduction to the Cost-Efficient Home Automation System (CEHA)

The extensive use of electronic devices and ineffective energy management techniques are the main causes of the worlds rising energy consumption. This projects goal is to use the VSDSquadron Mini RISC-V board to create a Cost-Effective IoT-Based Home Automation System in order to solve this problem. Users will be able to automate chores remotely operate household appliances and keep an eye on energy usage with this system which will ultimately improve comfort and convenience while cutting down on energy waste. The purpose of this project is to show how the RISC-V platform can be used to develop creative and reasonably priced smart home solutions by utilizing its open source nature and availability.


# Overview of (CEHA)

Designing and implementing a home automation system with the VSDSquadron Mini RISC-V board as its central processing unit is the suggested solution. This system will smoothly incorporate a range of communication, actuators, and sensors. modules that make it possible to monitor and control household appliances. Notable features include energy consumption tracking, automation scheduling, remote operation, and security features. The system will be accessible to users through a user-friendly web interface or mobile application.

The major objective is to use the VSDSquadron Mini RISC-V board to create an IoT-based home automation system that is both inexpensive and useful. For practical Internet of things applications this includes developing a system that can manage a range of household appliances and showcasing the RISC-V architectures affordability and capabilities.

This project has a number of important features and advantages:-
1) First off, the system is incredibly economical thanks to the open-source software and inexpensive VSDSquadron Mini RISC-V board. 
2) Second, because it is open-source, a wide range of devices and features can be integrated and customized. By enabling remote control of appliances, automating chores, and customizing comfort settings, it also improves user convenience.
3) Crucially, the system encourages energy efficiency with features like occupancy-based lighting control and smart thermostats. Lastly, it supports the expansion and advancement of the RISC-V ecosystem.

# Working of (CEHA) System

1. Power Supply: The ESP32 module, DHT11, PIR, Touch sensors, relay module, and VSDSquadron Mini board all receive the required power from the 5V power supply. Appliances connected to the relay can have their AC mains power controlled by the AC Mains to Supply Power with Relay circuit. 

2. Acquisition of Sensor Data: -Temperature and humidity are measured by the DHT11 sensor. This information can be used to control appliances based on temperature (e.g., adjusting fan speed based on temperature). 
-Motion is detected by aaPIR sensor. Actions such as turning lights on when motion is detected and off after a predetermined amount of inactivity can be triggered by this. 
-Touch Sensor: Enables manual device control or the activation of particular actions through touch input.

3. Data Processing and Management: Data from the sensors (DHT11, PIR, Touch) is read by the VSDSquadron Mini. makes decisions by processing the sensor data (e.g., adjusting fan speed based on temperature, turning lights on/off based on PIR sensor input). It Transmits and receives commands by communicating with the ESP32 module. Data is received by the ESP32 Module from the VSDSquadron Mini. uses Wi-Fi to connect to the internet. sends information to the cloud (like the Arduino IoT Cloud) for remote access and storage. gets commands for control from the mobile app or the cloud. sends commands to the VSDSquadron Mini for control.

4. Appliance Control: The VSDSquadron Mini sends control signals to the relay module. Depending on the signals it receives, switches turn on and off the power to the connected appliances (lights, fans, etc.).

5. Control and User Interface: The Arduino IoT Remote mobile app allows users to communicate with the system. Track sensor data in real time (temperature, humidity). Remotely control appliances (fan speed, light on/off, etc.). Plan automated tasks, such as turning on lights at dusk.

6. Cloud-Based Communication: Users can access and monitor system data remotely thanks to the ESP32 module's data transmission to the cloud. Additionally, the cloud can offer insights into patterns of energy consumption and store historical data for analysis.


Hence, Overall this "Cost-Effective IoT-Based Home Automation System" functions as: The brain of the system, the VSDSquadron Mini board, gathers information from sensors such as motion, temperature, and humidity. After processing this data, it makes choices like turning on lights when it detects motion or modifying fan speed in response to temperature. Through data transmission to the cloud for remote monitoring and command reception from the user interface (web/mobile app), the ESP32 module enables communication. The VSDSquadron Mini receives these commands and uses them to control the relay module that turns appliances on and off. Through the web interface or mobile app, users communicate with the system, scheduling automated actions, managing devices, and monitoring data. This integrated system offers a practical and economical way to control household appliances.

# Features and Benefits of ( CEHA )

a) It Controls the energy management and consumption with power monitoring of all the devices. It controls all the home appliances from the remote directly. So, it is the Remote Control based System which can control the devices from anywhere at anytime easily and making life easier for the individual . 
b) The solution also helps in reducing manual effort and improves efficiency . 
c) This system also optimizes temperature and saving Energy . 
d) It also reduces the cost of the bills and tracks unnecessary usage of the energy which leads to identifying more areas for improvements in energy saving . 
e) This system uses low-cost sensors to track and control the functioning of home/offices appliances for example, Light, Fan,etc. from the remote .

## Some other Key-Features are :- 

- Reducing energy consumption and saving wastage of energy monitoring: This solution is helpful for Person with Disbailities , as they can use remote for controlling the home appliances. 

-Cost-Effectiveness: The implementation of a cost-efficient, open-source hardware architecture (VSD mini RISC-V) enhances the economic feasibility of the system.  -Flexibility: The open-source framework of RISC-V permits extensive customization and fosters the creation of a diverse array of features and integrations.  

-Innovation: This initiative contributes to the expansion of the RISC-V ecosystem and promotes the advancement of novel and inventive home automation solutions. 

-Budget-Friendly: This solution is budget friendly in making this project , as , all the appliance become fully automated, so it makes it easy to control and come under budget as, only sensors are used for making the devices to control automatically. 

-User-Friedly: Any user can use it easily and can control automatically all devices with the help of remote as it interface with the app and wifi module.

# List of Components Required for CEHA System


| Item    | Quantity |
|---------|-----|
|AC Mains Power Supply     | 1  | 
|  4-Channel Relay   | 1  | 
|VSDSquadron mini| 1|
| ESP32 MODULE | 1  |  |
| Touch Sensor | 1 | Display |
| Connecting wires | 1Set |
|2 CH relay5V -240V|1|
| Touch Sensor | 1|
|5v-voltage regulator adaptor| 1|
| Zero PCB | 1|
|Switch | 1 |
| LED bulb | 2|
| Small Fan | 1|
| DHT11 Sensor | 1|
| Case box | 1|

# PIN OUT TABLE  

|Component     	|    Pin/Connection	 |     Connected To|
|----------------|--------------------|-----------------|
|Energy Meter  	|Pulse Output	   |   Optocoupler (Input)|
|Optocoupler(4N35)|	Input	Energy Meter |Pulse Output|
|                 |Output	|VSDSquadron mini GPIO Input Pin (PD2)|
|                |                  |                   |	
|VSDSquadron mini|	GPIO Pin (PD2) 	|LM393 input|
|                |GPIO Pin TX (PD5)|	GPIO Pin RX (16)|
|                | GPIO Pin RX (PD6)|	GPIO Pin TX (17)|
|                |                   |                  |
|ESP32		       |                   |                  |
|                | RX (16)        	|VSDSquadron mini TX (PD5)|
|	        |TX (17)	|VSDSquadron mini RX (PD6)|
|               |              |                          |
|Relay module	|Signal pin	|VSDSquardron mini GPIO Pin PC3|
|               |Vcc	|3.3V/5V (depending on relay)   |
|               |	GND    |	GND            |
|	        |COM	|Power Line (Common)           |
|               |	NO (Normally Open)|	Load(Device Being Controlled)|
|               |	NC (Normally Closed)|	Optional (for fail-safe connections)|
|                |                          |                                       |	
|5 volt adaptaor | 	Phase	|Phase of the energy meter                 |
|                 |	Netural |	Netural of the energy meter         |
|             |	5V	  |VSDSquadron mini|  VCC                                    |
|              |	GND	|VSDSquadron mini | GND                    |                 
|LM393 Comparator |D0      |  VSDSquadron mini   GPIO PD6                |
|                 |5V       |VSDSquadron mini 5V|
|                 |         |VSDSquadron mini GND|
|I2C LCD |	SDA|	vsdsquadron mini GPIO (PC1)|
|            |SCA|	vsdsquadron mini GPIO (PC2)|


# BLOCK DIAGRAM OF THE CEHA SYSTEM 

![block diagram CEHA ](https://github.com/user-attachments/assets/f5a8357d-9aba-4cc0-890a-ebbfae2a339f)

# CIRCUIT DIAGRAM OF CEHA SYSTEM

![circuit diagram of CEHA](https://github.com/user-attachments/assets/339c1629-1405-4375-97f7-8114d61c4cf0)


