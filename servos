#include<Servo.h>

Servo s1;
Servo s2;
Servo s3;
Servo s4;
Servo s5;
Servo s6;
Servo s7;
Servo s8;
Servo s9;
Servo s10;
Servo s11;
Servo s12;
Servo s13;
Servo s14;
Servo s15;



int angle = 0; // pannel position
int lightSensorPin = A1; // light sensor
int lightSensorValue = 0; // light sensor value
int targetAngle = 0;

void setup() {
  s1.attach(38);
  s2.attach(53);
  s3.attach(50);
  s4.attach(49);
  s5.attach(41);
  s6.attach(37);
  s7.attach(46);
  s8.attach(45);
  s9.attach(42);
  s10.attach(34);
  s11.attach(32);
  s12.attach(30);
  s13.attach(26);
  s14.attach(24);
  s15.attach(22);
  


  Serial.begin(9600);
}

void loop() {

  lightSensorValue = analogRead(lightSensorPin); // reads the value in the sensor

  targetAngle = map(lightSensorValue, 200 , 1023, 0, 45); // maps the value to 0 - 120 for the position of the servo

  /*if (angle < targetAngle) {
    while (s1.read() < targetAngle) {
      s1.write(angle);
      s2.write(angle);
      s3.write(angle);
      s4.write(angle);
      s5.write(angle);
      s6.write(angle);
      s7.write(angle);
      s8.write(angle);
      s9.write(angle);
      s10.write(angle);
      s11.write(angle);
      s12.write(angle);
      s13.write(angle);
      s14.write(angle);
      s15.write(angle);
      angle++;
      delay(100);
    }
    }

    if (angle > targetAngle) {
    while (s1.read() > targetAngle) {
      angle--;
      s1.write(angle);
      s2.write(angle);
      s3.write(angle);
      s4.write(angle);
      s5.write(angle);
      s6.write(angle);
      s7.write(angle);
      s8.write(angle);
      s9.write(angle);
      s10.write(angle);
      s11.write(angle);
      s12.write(angle);
      s13.write(angle);
      s14.write(angle);
      s15.write(angle);
      delay(100);
    }
    }
*/
  for (int i = 0; i < 46; i++) {
    s1.write(i);
    s2.write(i);
    s3.write(i);
    s4.write(i);
    s5.write(i);
    s6.write(i);
    s7.write(i);
    s8.write(i);
    s9.write(i);
    s10.write(i);
    s11.write(i);
    s12.write(i);
    s13.write(i);
    s14.write(i);
    s15.write(i);
    delay(200);
  }
    for (int i = 46; i > 0; i--) {
    s1.write(i);
    s2.write(i);
    s3.write(i);
    s4.write(i);
    s5.write(i);
    s6.write(i);
    s7.write(i);
    s8.write(i);
    s9.write(i);
    s10.write(i);
    s11.write(i);
    s12.write(i);
    s13.write(i);
    s14.write(i);
    s15.write(i);
    delay(200);
  }
 /* s1.write(0);
  s2.write(0);
  s3.write(0);
  s4.write(0);
  s5.write(0);
  s6.write(0);
  s7.write(0);
  s8.write(0);
  s9.write(0);
  s10.write(0);
  s11.write(0);
  s12.write(0);
  s13.write(0);
  s14.write(0);
  s5.write(0);*/


  Serial.print(lightSensorValue);
  Serial.print(",");
  Serial.print(angle);
  Serial.print(",");
  Serial.print(targetAngle);
  Serial.print(",");
  Serial.println(s1.read());
}
