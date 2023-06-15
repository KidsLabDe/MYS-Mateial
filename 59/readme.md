# Tasten und der Arduino

Um die Tasten direkt an den Arduino anzuchließen, brauchst Du entweder einen Wiederstand.
Entweder mit einem "echten" und einer kleine Schaltung, oder Du kannst den internen Pull-Up Widerstand im Arduino nutzen. 
Ohne Widerstand kommt nur Müll raus und der Schalter im Code springt immer hin und her. 

## Variante 1: Interner Widerstand (empfohlen)

´´´
pinMode(2,INPUT_PULLUP);
int sensorValue = digitalRead(2);
´´´



## Variante 2: Externen Widerstand

![](https://www.seeedstudio.com/blog/wp-content/uploads/2020/02/image-39.png)


# Links und Infos

Genauer erkärt wird das ganze in diesem schönen Artikel von Seeed:

https://www.seeedstudio.com/blog/2020/02/21/pull-up-resistor-vs-pull-down-differences-arduino-guide/
