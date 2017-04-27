# ColorMxingLamp
const int redLEDPin = 9;
const int redSensorPin = AO;
int red value = 0;
int green value = 0;
int blue value = 0;

int redSensorValue = 0;
int greenSensorValue = 0;
int blueSensorValue = 0;

void setup() {
  Serial.begin(9600);
  // put your setup code here, to run once:

}

void loop() {
  // put your main code here, to run repeatedly:
redSensorValue = analogRead(redSensorPin);
delay(5);

Serial.print("Raw Sensor Values/t Red: ");
Serial.print(redSensorValue);
delay(2000);

Seial.print("\t Green: ");
Serial.print(greenSensorValue);
delay(2000);

Serial.print("\t Blue: ");
Serial.println(blueSensorValue);
delay(2000);

redValue = redSensorValue/4;
greenValue = greenSensorValue/4;
blueValue = blueSensorValue/4:

Serial.print("Mapped Sensor Values \t Red: ");
Serial.print(redValue);

Serial.print("\t Green: ");
Serial.print(greenValue);

Serial.print("\t Blue: ")
Serial.println(blueValue);

analogWrite(redLEDPin, redValue);
analogWrite(greenLEDPin, greenValue);
analogWrite(blueLEDPin, blueValue);3
}
