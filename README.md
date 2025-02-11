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

1. Power Supply: The ESP32 module, PIR, Touch sensors, relay module, and VSDSquadron Mini board all receive the required power from the 5V power supply. Appliances connected to the relay can have their AC mains power controlled by the AC Mains to Supply Power with Relay circuit. 

2. Acquisition of Sensor Data: 
-Motion is detected by aaPIR sensor. Actions such as turning lights on when motion is detected and off after a predetermined amount of inactivity can be triggered by this. 
-Touch Sensor: Enables manual device control or the activation of particular actions through touch input.

3. Data Processing and Management: Data from the sensors ( PIR, Touch) is read by the VSDSquadron Mini. makes decisions by processing the sensor data (e.g.,  turning lights on/off based on PIR sensor input). It Transmits and receives commands by communicating with the ESP32 module. Data is received by the ESP32 Module from the VSDSquadron Mini. uses Wi-Fi to connect to the internet. sends information to the cloud (like the Arduino IoT Cloud) for remote access and storage. gets commands for control from the mobile app or the cloud. sends commands to the VSDSquadron Mini for control.

4. Appliance Control: The VSDSquadron Mini sends control signals to the relay module. Depending on the signals it receives, switches turn on and off the power to the connected appliances (lights, fans, etc.).

5. Control and User Interface: The Arduino IoT Remote mobile app allows users to communicate with the system. Track sensor data in real time . Remotely control appliances (fan speed, light on/off, etc.). Plan automated tasks, such as turning on lights at dusk.

6. Cloud-Based Communication: Users can access and monitor system data remotely thanks to the ESP32 module's data transmission to the cloud. Additionally, the cloud can offer insights into patterns of energy consumption and store historical data for analysis.


Hence, Overall this "Cost-Effective IoT-Based Home Automation System" functions as: The brain of the system, the VSDSquadron Mini board, gathers information from sensors such as motion, . After processing this data, it makes choices like turning on lights when it detects motion . Through data transmission to the cloud for remote monitoring and command reception from the user interface (web/mobile app), the ESP32 module enables communication. The VSDSquadron Mini receives these commands and uses them to control the relay module that turns appliances on and off. Through the web interface or mobile app, users communicate with the system, scheduling automated actions, managing devices, and monitoring data. This integrated system offers a practical and economical way to control household appliances.

# Features and Benefits of ( CEHA )

a) It Controls the energy management and consumption with power monitoring of all the devices. It controls all the home appliances from the remote directly. So, it is the Remote Control based System which can control the devices from anywhere at anytime easily and making life easier for the individual . 
b) The solution also helps in reducing manual effort and improves efficiency . 
c) This system also optimizes temperature and saving Energy . 
d) It also reduces the cost of the bills and tracks unnecessary usage of the energy which leads to identifying more areas for improvements in energy saving . 
e) This system uses low-cost sensors to track and control the functioning of home/offices appliances for example, Light, Fan,etc. from the remote .

## Some other Key-Features are :- 

- Reducing energy consumption and saving wastage of energy monitoring: This solution is helpful for Person with Disbailities , as they can use remote for controlling the home appliances. 

-Cost-Effectiveness: The implementation of a cost-efficient, open-source hardware architecture (VSD mini RISC-V) enhances the economic feasibility of the system.  

-Flexibility: The open-source framework of RISC-V permits extensive customization and fosters the creation of a diverse array of features and integrations.  

-Innovation: This initiative contributes to the expansion of the RISC-V ecosystem and promotes the advancement of novel and inventive home automation solutions. 

-Budget-Friendly: This solution is budget friendly in making this project , as , all the appliance become fully automated, so it makes it easy to control and come under budget as, only sensors are used for making the devices to control automatically. 

-User-Friedly: Any user can use it easily and can control automatically all devices with the help of remote as it interface with the app and wifi module.

# List of Components Required for CEHA System


| Item    | Quantity |
|---------|-----|
|AC Mains Power Supply     | 1  | 
|VSDSquadron mini| 1|
| ESP32 MODULE | 1  |  |
| Connecting wires | some Set |
| Touch Sensor | 2|
|5v-voltage regulator adaptor| 1|
| Zero PCB | 1|
| LED bulb | 3|
| Case box | 1|

# PIN OUT TABLE  


| **Component**          | **Pin/Connection**   | **End Point Connected To**                           |
|-----------------------|--------------------|------------------------------------------|
| **ESP32**              | 19                 |PC5  vsdsquadronmini                     |
|                        | 18                 |PC6  vsdsquadronmini                     |
| **5V Adapter**        | Power             | Power to whole CEHA SYstem                  |
|                        | 5V                 | VSDSquadron Mini & ESP32 VCC              |
|                        | GND                | VSDSquadron Mini & ESP32 GND              |
| **Touch Sensor 1**     | GPIO                | VSDSquadron Mini GPIO PD2                |
|                        | VCC                 | VSDSquadron Mini 3V                      |
|                        | GND                | VSDSquadron Mini GND                      |
| **Touch Sensor 2**     | GPIO                 | VSDSquadron Mini GPIO PD3               |
|                        | VCC                 | VSDSquadron Mini 3V                      |
|                        | GND                | VSDSquadron Mini GND                     |
| **PIR Sensor**         | D0                 | VSDSquadron Mini GPIO (PD5)              |                  
|                        | VCC                 | VSDSquadron Mini 5V                      |
|                        | GND                | VSDSquadron Mini GND                     |
|  **LED1**              |SIGNAL              |VSDSquadron Mini PD4                      |
|                        | GND                | VSDSquadron Mini GND                     |
|  **LED2**              |SIGNAL              |VSDSquadron Mini PC3                      |
|                        | GND                | VSDSquadron Mini GND                     |
|  **LED3**              |SIGNAL              |VSDSquadron Mini PC4                      |
|                        | GND                | VSDSquadron Mini GND                     |



# BLOCK DIAGRAM OF THE CEHA SYSTEM 

![Copy of Blank diagram](https://github.com/user-attachments/assets/3db11dc7-3e94-4b82-af0e-06d51edc2ca8)




# CIRCUIT DIAGRAM OF CEHA SYSTEM

![CKT](https://github.com/user-attachments/assets/fb5ac66b-e984-4b5a-bac3-fddc5b9eabf7)


# Introduction to Arduino IOT Cloud

The Arduino IoT Cloud is an integrated platform designed to facilitate the development and deployment of IoT projects. It enables seamless connectivity and device management providing users with remote control and project monitoring. The projects backbone is the Arduino IoT Cloud which connects the smart energy meter to the internet and enables remote control and real-time data visualization. Because of the Arduino IoT Clouds intuitive interface we can design and manage IoT devices with it. The platform supports many Arduino boards including the popular ESP32 and MKR series which are perfect for Internet of Things applications. The Arduino IoT Cloud allows us to define attributes like cost energy consumption and relay states. These properties have been updated.



# SOURCE CODE OF VSDSQUARDRON MINI AND ESP32 


### Code for VSDSQuadron Mini
``` 
VSDSquadron Mini code 


#define TOUCH_SENSOR_1  PD2
#define TOUCH_SENSOR_2  PD3
#define OUTPUT_1        PD4
#define OUTPUT_2        PC3

#define ESP_CTRL_1      PC5  // ESP32 control pin for Light 1
#define ESP_CTRL_2      PC6  // ESP32 control pin for Light 2

#define PIR_SENSOR      PD5  // PIR sensor input
#define OUTPUT_3        PC4  // New LED output controlled by PIR sensor

//int pirState = 0;
bool light1 = false;
bool light2 = false;
bool lastTouch1State = LOW;
bool lastTouch2State = LOW;
bool lastESP1State = LOW;
bool lastESP2State = LOW;

void setup() {
    pinMode(TOUCH_SENSOR_1, INPUT);
    pinMode(TOUCH_SENSOR_2, INPUT);
    pinMode(PIR_SENSOR, INPUT);

    pinMode(OUTPUT_1, OUTPUT);
    pinMode(OUTPUT_2, OUTPUT);
    pinMode(OUTPUT_3, OUTPUT);

    pinMode(ESP_CTRL_1, INPUT);
    pinMode(ESP_CTRL_2, INPUT);
}

void loop() {
    // Read touch sensor 1 state
    bool currentTouch1State = digitalRead(TOUCH_SENSOR_1);
    if (currentTouch1State == HIGH && lastTouch1State == LOW) {
        light1 = !light1;  // Toggle light
        digitalWrite(OUTPUT_1, light1);
        delay(300);  // Debounce delay
    }
    lastTouch1State = currentTouch1State;

    // Read touch sensor 2 state
    bool currentTouch2State = digitalRead(TOUCH_SENSOR_2);
    if (currentTouch2State == HIGH && lastTouch2State == LOW) {
        light2 = !light2;  // Toggle light
        digitalWrite(OUTPUT_2, light2);
        delay(300);  // Debounce delay
    }
    lastTouch2State = currentTouch2State;

    // Read ESP32 control 1 state
    bool currentESP1State = digitalRead(ESP_CTRL_1);
    if (currentESP1State == HIGH && lastESP1State == LOW) {
        light1 = !light1;  // Toggle light
        digitalWrite(OUTPUT_1, light1);
        delay(300);
    }
    lastESP1State = currentESP1State;

    // Read ESP32 control 2 state
    bool currentESP2State = digitalRead(ESP_CTRL_2);
    if (currentESP2State == HIGH && lastESP2State == LOW) {
        light2 = !light2;  // Toggle light
        digitalWrite(OUTPUT_2, light2);
        delay(300);
    }
    lastESP2State = currentESP2State;

    // Read PIR sensor state
    int pirState = digitalRead(PIR_SENSOR);
    if (pirState == HIGH) {
        digitalWrite(OUTPUT_3, HIGH);  // Turn on new LED
    } 
    else {
        digitalWrite(OUTPUT_3, LOW);   // Turn off new LED
    }
}



////////////////////////////////////////////////////////

```
### Code for ESP32 Module 
``` 
Esp32 code 

#include "thingProperties.h"

#define LIGHT_1_CTRL 18  // GPIO for Light 1 control
#define LIGHT_2_CTRL 19  // GPIO for Light 2 control

void setup() {
    Serial.begin(115200);
    initProperties();
    ArduinoCloud.begin(ArduinoIoTPreferredConnection);
    
    pinMode(LIGHT_1_CTRL, OUTPUT);
    pinMode(LIGHT_2_CTRL, OUTPUT);
}

void loop() {
    ArduinoCloud.update();

    // Control VSDSquadron Mini via GPIOs
    digitalWrite(LIGHT_1_CTRL, light1_state);
    digitalWrite(LIGHT_2_CTRL, light2_state);
}

/*
  Since Light1State is READ_WRITE variable, onLight1StateChange() is
  executed every time a new value is received from IoT Cloud.
*/
void onLight1StateChange()  {
  // Add your code here to act upon Light1State change
}
/*
  Since Light2 is READ_WRITE variable, onLight2Change() is
  executed every time a new value is received from IoT Cloud.
*/
void onLight2Change()  {
  // Add your code here to act upon Light2 change
}
/*
  Since Light2State is READ_WRITE variable, onLight2StateChange() is
  executed every time a new value is received from IoT Cloud.
*/
void onLight2StateChange()  {
  // Add your code here to act upon Light2State change
}



```

# Functionality 

Functionality of the CEHA :-

1.	Touch-Based Control:
     •	The system includes two touch sensors interfaced with the VSDSquadron Mini, which act as input triggers.
     •	When a touch sensor is activated, the corresponding LED lights up.
2.	Motion Detection:
     •	A PIR sensor is integrated to detect motion.
     •	When motion is detected, another LED automatically turns on, enhancing security and convenience.
3.	Wi-Fi-Based Remote Control:
     •	An ESP32 acts as a secondary board, enabling remote control.
     •	The two LEDs can be triggered wirelessly through Arduino Cloud Dashboard, allowing users to operate the system from anywhere using Wi-Fi.
This project combines cost efficiency, smart automation, and remote access, making it a practical solution for modern home automation.

# IMAGE OF THE Final Product

![ceha image ](https://github.com/user-attachments/assets/4518afcf-7f91-4ff0-ad3a-3323263ebead)

# Demonstration Video of the Product working  


https://github.com/user-attachments/assets/4a794490-5865-4092-aeec-8f5c500ca96d

# Demonstration Video of Final Product

Please click on the below link, to see the full demonstration of final product.....----

https://drive.google.com/file/d/1mKWnLduUi8WlkTlkoxxfBus3ZQWCTpxj/view?usp=sharing



# Conclusion

This project effectively illustrated the viability of using the VSDSquadron Mini RISC-V board to create an affordable and useful Internet of Things-based home automation system. Remote control, automated scheduling, energy monitoring, and basic security features were all made possible by the system's integration of several sensors and actuators. The cost effectiveness of the solution was enhanced by the utilisation of open-source software and the open-source RISC-V board. This project demonstrates how the RISC-V architecture may be used to develop creative and approachable smart home solutions. 

The main accomplishments are highlighted in this conclusion: 
- Functional System: A home automation system that functions and has the functionality that 
users want. 
- Cost-Effectiveness: Attained by utilising the inexpensive RISC-V board. 
- RISC-V Potential: Exhibited the RISC-V architecture's potential for Internet of Things 
applications.

# Acknowledgements

* [Kunal Ghosh](https://github.com/kunalg123), Co-founder, VSD Corp. Pvt. Ltd.


## Author


- [Vanshika Tanwar](https://github.com/VanshikaTanwar), Bachelor of Technology in Electronics & Communication Engineering,Dronacharya Group of Institutions,Greater Noida, U.P.


