# Disaster-Zone-People-Detection-System
## Overview
The prototype is designed to assist in locating and counting people trapped in a room during a natural calamity. It employs PIR sensors, FSR sensors, GPS, and ESP32 microcontrollers to detect the number of people and transmit data via Bluetooth. The receiver then displays this information, including the location coordinates, on an LCD, enabling rescuers to act efficiently.

## Transmitter Unit
The transmitter unit is responsible for counting the number of people in a room and triggering data transmission, including their coordinates, during a natural calamity.

### 1) Components:

#### * PIR Sensors: 
Installed at the entrance and exit to count the number of people entering and leaving the room.

#### * FSR Sensor:
Detects pressure caused by distress during a calamity, such as individuals pressing it under debris.

#### * GPS Module: 
Provides the location coordinates of the room where people are trapped.

#### * ESP32 Microcontroller: 
Acts as the main processing unit, storing the count of people and fetching the location coordinates from the GPS module.

#### * Bluetooth Module (Built into ESP32): 
Transmits the stored data when triggered by the FSR sensor.

### 2) Working:
* The PIR sensors continuously track people entering and exiting the room, maintaining a real-time count.

#### During a natural calamity, if the FSR sensor detects pressure (indicating someone is in distress), it triggers the ESP32 to broadcast the following data:
* Number of people currently in the room.
* Coordinates of the room’s location from the GPS module.
* This data is sent via Bluetooth to nearby receivers.

### Receiver Unit
The receiver unit is designed to collect transmitted data and display it for rescuers during a natural calamity.

#### 1) Components:
* ESP32 Microcontroller: Receives Bluetooth transmissions from the transmitter.
* LCD Display: Displays the number of people trapped and their location coordinates.

#### 2) Working:
* When the receiver comes within range of the transmitter’s Bluetooth signal, the ESP32 processes the received data.
* The data, including the count of trapped individuals and their GPS coordinates, is displayed on the LCD screen, allowing rescuers to locate and assist those in need efficiently.

## Conclusion
This system is a comprehensive solution for identifying and locating individuals trapped during natural calamities such as earthquakes, landslides, or floods. It leverages PIR sensors for accurate people counting, an FSR sensor for emergency distress detection, a GPS module for precise location tracking, and Bluetooth technology for wireless communication. By providing both the number of people trapped and their exact location, this prototype ensures faster and more effective rescue operations.



https://github.com/user-attachments/assets/d595eae3-1ef3-4b47-95c7-f0839c5bcc91

