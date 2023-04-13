# 3.5
float R1=100000;


float R2=100000;

void setup()
{
  Serial.begin(9600);
}
void loop()
{
float v=(analogRead(A0)*5)/1023.0;
float Resultado=(v/(R2/(R1+R2)));
Serial.print("v= ");
Serial.println(Resultado);
delay(500);
}
