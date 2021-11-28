int convertValue;
int ledPin = 11;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  convertValue = analogRead(A0);
  analogWrite(ledPin, map(convertValue, 0, 1023, 0, 255));
}
