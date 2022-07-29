# Digital-Analog-sensors
Examples on Digital analog sensors

# Digital-Sensor

The digital pins on the Arduino provide a 1-bit signal (HIGH or LOW).have different types one is PIR sensor, which the project is  about.
PIR (passive infrared)  This type of emission is not visible to the human eye, but sensors that operate using infrared wavelengths can detect such activity. They are sometimes referred to as ‘motion-based detectors’, as they sense the presence of people, animals and objects through the movement of their infrared wavelengths.

project component
1.arduino
2.led 
3.resistor 
4.breadboard
5.PIR sensor
connected as shown in the picture
![Screenshot (1080)](https://user-images.githubusercontent.com/108452991/181682332-1adfadd3-3c89-4f58-9095-981942bc94fb.png)

and the code is :
int PIRsensor = 0;
void setup() {
  pinMode(11, INPUT);
  pinMode(9, OUTPUT);
}

void loop() {
  PIRsensor = digitalRead(11);
  if(PIRsensor == HIGH) {
    digitalWrite(9, HIGH);
     }
  else{
    digitalWrite(9,LOW);
   }
}

try it!
https://www.tinkercad.com/things/devEIQ7cCXj


