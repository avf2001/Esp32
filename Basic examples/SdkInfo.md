```c
void setup() {
  Serial.begin(115200);
  Serial.println("SDK");
  Serial.println(ESP.getSdkVersion());
  Serial.println("SDK через низкоуровневую функцию:");
  Serial.println(esp_get_idf_version());
}

void loop() {}
```
