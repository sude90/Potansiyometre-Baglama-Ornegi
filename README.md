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
![potansiyometre bağlanış](https://user-images.githubusercontent.com/78275279/205259325-54efd701-4ba5-436a-96e3-456020bd41bb.PNG)
