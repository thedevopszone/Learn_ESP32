# Learn ESP32


## Blink

```
int LED_BUILTIN = 1;

void setup() {
  pinMode (LED_BUILTIN, OUTPUT);
}


void loop() {
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000);
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000);
}


```

