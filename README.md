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



## WLAN

```
#include "WiFi.h"

const char * ssid = "yourNetworkName";
const char * password = "yourNetworkPass";

void setup() {
  Serial.begin(9600);
  WiFi.begin(ssid, password);
  while (WiFi.status() != WL_CONNECTED) {
    delay(500);
    Serial.println("Connecting to WiFi..");
  }
  Serial.println("Connected to the WiFi network");
}

void loop() {}
```

