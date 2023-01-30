# Covid_Risk_Monitor

## **Project Description**
The idea of this project is to design an IoT device that monitors a user’s covid risk level based on their daily activities and interactions. This device will make it easier for users to abide by the Public Health covid-19 guidelines and prevent rapid growth of covid-19 cases. The device will detect other humans through their emitted energy (electromagnetic radiation) and read their temperature. We also keep track of their distance (at least two meters) with our user. This device will also keep track of the user's location,which will allow the user to see who they might have been in contact with. This way if one user tests positive, we can alert other users who were at the same location about a potential exposure to covid-19. Taking into account all the data gathered through the day, the user will be notified of their risk level or get an exposure warning. 

## Components
Data by the sensors and sent to raspberry pi, the raspberry pi then sends the data trhough a payload to IoT hub. The data is sent every two seconds to the IoT Hub and displayed to the user. (Code in SensorToCloud.py file)

## Technologies Used 
- Python
- Raspberry Pi
- Azure Cloud
- Power BI Data Visualization
