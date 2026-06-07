# Motion Detection Security Alarm

Team Members: Afreen, Nishitha, Archa

To design a motion detection security alarm system using Arduino that can sense human movement and activate an alarm or light as a security alert. The system aims to enhance home and office safety by providing a simple, low-cost, and reliable intrusion detection method.

Components:
Arduino Uno R3
,Breadboard 400 Tie Points
,Buzzer 9v-12v Active
,Programming Cable for Arduino Uno & Mega
,PIR Motion Sensor
,Jumper Wires
,Red Leds
,Resistors-220 Ohm
,Software- Arduino IDE 2.3.6

Working: 
The PIR sensor detects motion by sensing changes in infrared radiation. When motion is detected,
it sends a HIGH signal to the Arduino. The Arduino then turns ON the buzzer and LED to alert the
user. After a short delay, both turn OFF, and the system returns to standby mode, ready to detect
motion again.

Cost Analysis:
Arduino board - Rs 390
PIR sensor - Rs 70
Breadboard - Rs 40
LED Lights - Rs 1
220Ω resistor - Rs 1
Buzzer - Rs 27
Standard USB A-to-B programming cable - Rs 35
Jumper wires(male-male and female-male) - Rs 16
Total Cost: Rs 580

Technical failures and it reasons:
False Alarms: The system has a high risk of false alarms as one in ten system alerts occur even when no motion is detected. Reason: High motion sensitivity to non-issue factors such as wind, swaying trees, curtains etc.

Outcomes:
The system successfully detects motion within the PIR sensor’s range (approximately 6–7 meters).
When motion is detected, both buzzer and LED turn ON for a few seconds alerting users that there has been motion detected.
The circuit returns to standby mode after the delay.
The project can be used for security or automatic light control.


<img width="1018" height="574" alt="image" src="https://github.com/user-attachments/assets/d9ffe43b-98bd-4249-a1e0-816e6207f030" />

<img width="606" height="772" alt="image" src="https://github.com/user-attachments/assets/7a0b68ac-d71d-44d8-b100-332ee60988d6" />

