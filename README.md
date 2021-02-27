# Arduino-Low-Power



## Duerme el arduino durante 8 segundos
```c++
#include "LowPower.h"

void setup()
{

}

void loop() 
{
  LowPower.powerDown(SLEEP_8S, ADC_OFF, BOD_OFF);
}

``` 

* Consume 30mA
* Apaga el Brown Out Detection y los convertidores de analogico a digital durante 8 segundos


