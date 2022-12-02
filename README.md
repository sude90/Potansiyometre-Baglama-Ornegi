# Potansiyometre-Baglama-Ornegi

void setup()
{
  pinMode(A0, INPUT);
  pinMode(2,OUTPUT);
  Serial.begin(9600);
}

void loop()
{
  
  int deger = analogRead(A0);
  if(deger > 420)
  {
    digitalWrite(2,1);
  }
  else if (deger < 420)
  {
    digitalWrite(2,0);
  }
  Serial.println(deger);
}
