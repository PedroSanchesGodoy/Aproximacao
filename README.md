# Aproximação Sensor

## Código

#include <EasyUltrasonic.h>


EasyUltrasonic sensor;


float distancia = 0;



void setup() {

Serial.begin(9600);

sensor.attach(18, 4, 2, 400);

}

void loop() {
distancia = sensor.getDistanceCM();
Serial.print(distancia);
Serial.println(" CM");

delay(1000);

}

## Foto
<img width="585" height="781" alt="image" src="https://github.com/user-attachments/assets/aa5c0dac-02ce-41b4-addd-6c5c72a6c85a" />

Fios:
Fio marrom nos 5 Volts
Fio Vermelho e fio cinza nas portas digitais
Fio laranja no Ground
