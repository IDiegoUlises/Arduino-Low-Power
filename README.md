# Arduino Low Power

![](https://github.com/IDiegoUlises/Arduino-Low-Power/blob/main/Images/Consumo-del-arduino-uno.gif)

* El Arduino consume 36mA en funcionamiento



## Duerme el arduino durante 8 segundos

![](https://github.com/IDiegoUlises/Arduino-Low-Power/blob/main/Images/Consumo-del-arduino-con-libreria.gif)

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

## Investigacion 

Arduino uno conectado en vin consume  
