Introduction:
This project presents an innovative approach to intruder detection leveraging computer vision 
integrated within the Cisco Packet Tracer simulation environment. As network security 
remains a critical concern, the ability to visually monitor and detect unauthorized access in 
real-time significantly enhances traditional network security measures. The proposed system 
utilizes computer vision to process live video feeds, identifying potential intruders through 
motion detection techniques. By incorporating this technology into Cisco Packet Tracer, a 
comprehensive simulation of both network traffic and physical security is achieved. This 
security framework allows network administrators to simulate, test, and refine their intrusion 
detection protocols within a controlled virtual environment. Our experimental results 
demonstrate the system’s efficiency in promptly detecting and alerting administrators to 
unauthorized access, thereby offering a robust tool for improving network security practices 
and training. 

Working: 
Our project is on intruder detection at home using Cisco Packet Tracer, incorporating a Home 
Gateway (DLG100), Siren, Motion Detector, CCTV, Lights , a representation of the front 
door, and a Control Tablet. The primary objective was to create a system that activates the 
siren and camera upon detecting motion, as well as turn on the lights and lock the doors for 
safety; and deactivates them when no motion is detected. Below is a detailed explanation of 
how we set up and configured the system, ensuring its proper functionality. 
The necessary components were the Home Gateway (DLG100), Motion Detector, Siren, 
Webcam (CCTV), Lights , the front door ,and Control Tablet. We connected all these devices 
to the Home Gateway using IoT custom cables to form a network. Then we configured each 
device. For the Home Gateway, we ensured it was powered on and connected to the network. 
For the Control Tablet, we configured it to ensure it was connected to the Home Gateway so 
that it can control the activities of the rest of the components. From here on the tablet is what 
controls and conditions the rest of the smart devices. To set the conditions for the system, we 
used the IoT Monitor in Cisco Packet Tracer coming under the controller . We used the 
conditions tab of the iot monitor to provide conditions upon which the siren goes off and web 
cam turns on. We basically added 2 conditions for the Motion Detector ,one to trigger the 
Siren and CCTV when motion is detected. The specific condition was set as follows: When 
the Motion Detector status is “ON”, the actions were to set both the Siren and CCTV statuses 
to “ON”. Additionally, we programmed another condition to handle the scenario when no 
motion is detected. This condition was: When the Motion Detector status is “OFF”, the 
actions were to set both the Siren and CCTV statuses to “OFF”. Additionally, we made the 
conditions so that, whenever a motion detector go off, it is to make sure that the lights turn on 
as well as the door stays locked. Once the motion detector is detecting no motion again, it 
goes back to safe state, where the lights re off and door is unlocked. To depict motion, we are 
using the ALT key and moving the cursor over the motion detector. This will trigger the 
detector making all the conditions above true and the actions follow. 
After setting these conditions, the system was tested by simulating motion within Cisco 
Packet Tracer. When the Motion Detector was triggered using the mouse/cursor, the Siren and 
CCTV turned on as expected. Conversely, when we simulated no motion, the Siren and 
CCTV turned off. This confirmed that the intruder detection system was working correctly. 
Through this project, we demonstrated the practical application of IoT devices in enhancing 
home security, showcasing the capability to detect intruders and respond accordingly with 
alerts and video recording. This simple application could further be improvised for larger 
security system, maybe by incorporating security passwords, or an alert message to the user 
whenever the alarm goes off etc. 
