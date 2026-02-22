# Motion-Detection-Security-Alarm
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

Code:
const int motionpin=A0;
const int ledpin=13;
const int buzzpin=12; // ledpin,motionpin and buzpin are not changed
throughout the process
int motionsensvalue=0;
void setup() {
Serial.begin(9600);
pinMode(ledpin, OUTPUT);
pinMode(motionpin,INPUT);
pinMode(buzzpin,OUTPUT);
}
void loop() {
motionsensvalue=analogRead(motionpin); // reads analog data from
motion sensor
if (motionsensvalue>=200){
digitalWrite(ledpin,HIGH);
tone(buzzpin,500); //turns on led and buzzer
}
else {
digitalWrite(ledpin,LOW); //turns led off led and buzzer
noTone(buzzpin);
}
}
