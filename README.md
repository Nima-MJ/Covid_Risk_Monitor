# Covid_Risk_Monitor

## **Project Description**
The purpose of this project is to create an IoT device that assesses a user's covid risk level based on their daily activities and interactions. The device will facilitate adherence to Public Health covid-19 guidelines and reduce the spread of the virus. It detects other people through electromagnetic radiation and measures their temperature, ensuring a safe distance of at least two meters with the user. The device also tracks the user's location to provide information about potential exposure to covid-19. Based on the collected data, the device informs the user of their risk level or issues an exposure warning.

## Components
The sensors gather data and send it to the Raspberry Pi, which then sends the information through a payload to the IoT Hub. This data is updated every two seconds and displayed to the user through the IoT Hub. The implementation of this process is included in the SensorToCloud.py file. For more detailed information, please refer to the [Project Design PDF](https://github.com/Nima-MJ/Covid_Risk_Monitor/blob/a3f31e51de76bcdb13b05ddeff201441e2caca76/src/Project%20Design.pdf) and [Project Proposal PDF](https://github.com/Nima-MJ/Covid_Risk_Monitor/blob/a3f31e51de76bcdb13b05ddeff201441e2caca76/src/Project%20proposal.pdf). 

## How to set it up
Setting up a Raspberry Pi according to the provided diagram involves both hardware and software tasks. Assemble the required components, connect GPIO pins as per the diagram, and install Raspbian OS on an SD card. After the initial boot and setup, update the OS, and install necessary packages such as RPi.GPIO for GPIO access and Azure IoT Device SDK for Azure integration. Create an Azure account, set up an IoT Hub service, and generate a connection key for device authentication. Modify the Python code to include the generated connection key, then run the script on the Raspberry Pi to collect data from sensors and send it to the Azure IoT Hub for processing. The exact steps and configurations may vary based on your project's specifics, so consulting relevant documentation is essential for a successful setup and data collection process.

## Technologies Used 
- Python: Used to gather the data from the GPIO pins and calculate the distance measured by the ultrasonic sensor using the pulse duration.
- Raspberry Pi 3 model B (Raspian OS): The GPIO pins were utilized to retrieve data and supply power to the sensors mounted on the breadboard.
- Libraries: Python Library, Raspberry Pi GPIO Library, the Azure IoT Device SDK (both the regular and asynchronous versions), gpsd-py3 for handling GPS data
- Sensors: GPS, PIR and Ultrasonic
- Azure Cloud IoT Hub, AMQP Protocol was used for communication 
- Power BI Data Visualization

![alt text](https://github.com/Nima-MJ/Covid_Risk_Monitor/blob/main/src/Project%20Design.png?raw=true)
![alt text](https://github.com/Nima-MJ/Covid_Risk_Monitor/blob/main/src/Layout.PNG?raw=true)
