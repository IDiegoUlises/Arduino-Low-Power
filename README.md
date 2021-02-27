# Arduino-Low-Power

Investigacion sobre disminuir el consumo energetico del arduino

## Codigo copiado de la liberia low power para prueba y mejorar
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

apunte consume 36MA arduino vacio sin codigo 
consume 36MA Ejecutando codigo

