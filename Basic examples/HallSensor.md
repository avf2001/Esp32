```c
const int LED = 1;

void setup() {
  Serial.begin(115200);
  pinMode(LED, OUTPUT);
}

void loop() {
  int sensor = hallRead();  // считываем показания датчика Холла
  Serial.print("Sensor Reading:");
  Serial.println(sensor);

  digitalWrite(LED, (sensor < 0) ? HIGH : LOW); // включаем светодиод при обнаружении магнита
  delay(500);
}
```
