# Arduino Low Power

![](https://github.com/IDiegoUlises/Arduino-Low-Power/blob/main/Images/Consumo-del-arduino-uno.gif)

* El Arduino consume 36mA en funcionamiento
* En el caso que se conecte a traves de vin consume 30mA



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
* * En el caso que se conecte a traves de vin consume 20mA

## Arduino sin la placa

Arduino consume 12mA en funcionamiento

Arduino con libreria power low consume 006.5 Ua microfaradios

