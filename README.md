#define PUL A3
#define FOQUITO 4
int lectura;
void setup() {
pinMode (PUL, INPUT);
Serial.begin(9600);
pinMode (FOQUITO, OUTPUT);
}
void loop() {
lectura = analogRead(PUL);
  Serial.println(lectura);
Serial.println(lectura);
delay(100);
if (lectura < 400){
  digitalWrite(FOQUITO,HIGH);
  }
if(lectura > 600){
  digitalWrite(FOQUITO,LOW);
  }
}
