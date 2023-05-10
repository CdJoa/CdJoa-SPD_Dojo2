
## Integrantes 
- Jonathan Fernandez
- Santiago Amato
- Joaquin Carnelos Duarte
- Magali Gimenez

## Descripción
La empresa “UTN FRA Robotics” ganó la licitación de un proyecto, y deberá
Implementar un sistema que permita al usuario saber a qué estación de subte está
llegando, aparte el sistema muestra las estaciones que faltan hasta llegar a destino,
para ello debemos utilizar 4 LEDs y el display de 7 segmentos. Esta vez el buzzer
deberá emitir un sonido diferente cada vez que se llegue a una estación.
El sistema deberá arrancar apagado, luego de presionar el botón empezará y hará lo
pedido.

1 - Parte Uno:(se entrega hoy)
Deberá mostrar los leds por estación y el número de estación en el display 7
segmentos.
2 - parte dos:(Próxima clase) sistema completo con el buzzer.

## Función principal:
#define A 8
#define B 7
#define C A1
#define D A2
#define E A3
#define F 6
#define G 5

#define LED_1 13
#define LED_2 12
#define LED_3 11
#define LED_4 10

void setup() {
  pinMode(LED_1, OUTPUT);
  pinMode(LED_2, OUTPUT);
  pinMode(LED_3, OUTPUT);
  pinMode(LED_4, OUTPUT);
  
  pinMode(A, OUTPUT);
  pinMode(B, OUTPUT);
  pinMode(C, OUTPUT);
  pinMode(D, OUTPUT);
  pinMode(E, OUTPUT);
  pinMode(F, OUTPUT);
  pinMode(G, OUTPUT);
  
  digitalWrite(LED_1, 0);
  digitalWrite(LED_2, 0);
  digitalWrite(LED_3, 0);
  digitalWrite(LED_4, 0);
  
  digitalWrite(A, 1);
  digitalWrite(B, 1);
  digitalWrite(C, 1);
  digitalWrite(D, 1);
  digitalWrite(E, 1);
  digitalWrite(F, 1);
  digitalWrite(G, 0);
}

void loop() {
  digitalWrite(LED_1, 1);
  digitalWrite(A, 1);
  digitalWrite(B, 1);
  digitalWrite(C, 1);
  digitalWrite(D, 1);
  digitalWrite(E, 1);
  digitalWrite(F, 1);
  digitalWrite(G, 0);
  delay(1000);
  digitalWrite(LED_1, 0);
  
  digitalWrite(LED_2, 1);
  digitalWrite(A, 1);
  digitalWrite(B, 1);
  digitalWrite(C, 1);
  digitalWrite(D, 1);
  digitalWrite(E, 1);
  digitalWrite(F, 1);
  digitalWrite(G, 0);
  delay(1000);
  digitalWrite(LED_2, 0);
  
  digitalWrite(LED_3, 1);
     digitalWrite(A, 1);
      digitalWrite(B, 1);
      digitalWrite(C, 1);
      digitalWrite(D, 1);
      digitalWrite(E, 0);
      digitalWrite(F, 0);
      digitalWrite(G, 1);
  
  delay(1000);
  digitalWrite(LED_3, 0);
  
  digitalWrite(LED_4, 1);
    digitalWrite(A, 0);
      digitalWrite(B, 1);
      digitalWrite(C, 1);
      digitalWrite(D, 0);
      digitalWrite(E, 0);
      digitalWrite(F, 1);
      digitalWrite(G, 1);
  delay(1000);
  digitalWrite(LED_4, 0);
  }
## Link al proyecto:
- [proyecto](https://www.tinkercad.com/things/geAwBPKdTkg?sharecode=WlrUgWZyVtcdrx5yOx2-e-REG3xwL3LwY6Pyq_x3qh4)
