# RobotCar
This project is developed by Team ¡VAMOS! for UTM AIROST Intern 24/25


**USER MANUAL**

  The robot car should be powered before use, which user needs to connect the two micro USB cables to the ESP32 and ESP32-Cam respectively and connect the Li-Ion batteries. After that, with the downloaded control app, user should connect Bluetooth to the name “ESP32_Robot” (Bluetooth should be TURNED ON before connect). If connected successfully, the label will be changed from “NOT CONNECTED” to “CONNECTED”. The Live Camera will be connected to the specified phone hotspot, and the setting can be set upon successful connection. With stream button in the WebBrowser clicked, there will be a live video. If connection unsuccessful, the ESP32-Cam should be reset by clicking the RST button, and click the Refresh Camera button to check whether connected or not. With all the connection done, click on the Manual button to start the manual control of the robot car. In manual mode, the car can be controlled by the movement buttons and the robotic arm will be activated as well. The robotic arm are controlled by adjusting the two sliders (Arm and Finger).
  
  To change to autonomous mode, simply click the Auto button. In autonomous mode, the movement buttons and robotic arm function will be disable, it will just follow the predefined line. For the predefined line, it can be setup using black tap with white background. (The line should not be complicated as this is two IR sensors module). The robot car follow the following logic in autonomous mode:
Line Follower Logic

1.Two IR sensors do not detect black line	Moving Forward

2.Left IR sensor detects black line only	Turn Left

3.Right IR sensor detects black line only	Turn Right

4.Two IR sensors detect black line 	Stop

If the robot car does not move with “beep” sound, user should push it so that it can have enough force to move forward.
