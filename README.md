# juego-de-luces
// el programa realiza un primer juego de luces,dos luces van encendiendo saltando una ,el segundo juego de luces enciendo un led saltando tres espacios y el tercer
//juego de luces enciende y apaga toda la tira de les en secuencia 

 //Jonathan Guerrero
 //20/10/2016
int contador1=0;// declaramos dos contadores inicializados en cero 
int contador2=0;
void setup() {
  // put your setup code here, to run once:
  pinMode (0, OUTPUT); //establecemos las salidas de los pines del arduino
  pinMode (1, OUTPUT);
  pinMode (2, OUTPUT);
  pinMode (3, OUTPUT);
  pinMode (4, OUTPUT);
  pinMode (5, OUTPUT);
  pinMode (6, OUTPUT);
  pinMode (7, OUTPUT);
  pinMode (8, OUTPUT);
  pinMode (9, OUTPUT);
  pinMode (10, OUTPUT);
  pinMode (11, OUTPUT);
  pinMode (12, OUTPUT);
  pinMode (13, OUTPUT);

  }
  void loop() {
      
    
  
for (contador1 = 1, contador2=0; contador1 < 14; contador1 = contador1 +4,contador2 = contador2 +4) {
      digitalWrite(contador1, HIGH);
      digitalWrite(contador2, HIGH);
      delay(200);
      digitalWrite(contador1,LOW);
      digitalWrite(contador2, LOW);
      delay(200);
         }
for (; contador1 < 14; contador1 = contador1 + 4)
    {
      digitalWrite(contador1, HIGH);
      delay(200);
    }

for (contador1 =14; contador1 >= 0; contador1 = contador1 - 4)
    {
      digitalWrite(contador1, HIGH);
      delay(200);
    }

    for ( ; contador1 < 14; contador1=contador1+4)
    {
      digitalWrite(contador1, LOW);
      delay(300);
    }
for (contador1 =14 ; contador1 >= 14; contador1=contador1-4) {
      digitalWrite(contador1, LOW);
      delay(300);
 }
     
for (contador1=0; contador1 < 14; contador1 ++)
    {
      digitalWrite(contador1, HIGH);
      delay(100);
    }

for (contador1 =0; contador1 <14; contador1 ++)
    {
      digitalWrite(contador1, LOW);
      delay(100);
    }
for ( contador1 =0; contador1 < 0; contador1++)
    {
      digitalWrite(contador1, HIGH);
      delay(100);
      }
for (contador1=0 ; contador1 <0; contador1++) {
      digitalWrite(contador1, LOW);
      delay(100);
       }
  }
   
