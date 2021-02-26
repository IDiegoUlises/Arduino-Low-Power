# Arduino-Low-Power

Investigacion sobre disminuir el consumo energetico del arduino

## Codigo copiado de la liberia low power para prueba y mejorar
```c++
#include "LowPower.h"

void setup()
{
  pinMode(13,OUTPUT);
}

void loop() 
{
  digitalWrite(13,HIGH);
  delay(2000);
  digitalWrite(13,LOW);
  LowPower.powerDown(SLEEP_2S, ADC_OFF, BOD_OFF);
}

``` 
