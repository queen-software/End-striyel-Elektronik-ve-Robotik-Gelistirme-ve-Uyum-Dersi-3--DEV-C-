# End-striyel-Elektronik-ve-Robotik-Gelistirme-ve-Uyum-Dersi-3--DEV-C++
## Formüller
v    = GERİLİM (VOLT)
I  =  AKIM
R  =  DİRENÇ

V = I * R        I = V / R

<img width="888" height="496" alt="image" src="https://github.com/user-attachments/assets/d9010cec-4bcf-4022-91e7-b88baeeb5312" />
<img width="848" height="598" alt="image" src="https://github.com/user-attachments/assets/d9665d15-ffd6-4ebe-9b5a-9fe2535832db" />
temp mail = sana bir tane mail verir
<img width="1519" height="781" alt="image" src="https://github.com/user-attachments/assets/82c8d427-17dc-41eb-8dd4-51337516f7ef" />
<img width="747" height="430" alt="image" src="https://github.com/user-attachments/assets/c0ef0854-7e3f-4b6a-929e-0db6063c8271" />

### Polis çakarı
<img width="1662" height="819" alt="image" src="https://github.com/user-attachments/assets/5b55202c-ddd6-425b-a91b-f8ae013eb2b1" />
###
    int kirmizi = 4;
    int mavi = 2;
    int yesil = 8;
    
    
    void setup()
    {
     
      pinMode(kirmizi,OUTPUT);
      pinMode(mavi,OUTPUT);
      pinMode(yesil,OUTPUT);
      Serial.begin(9600);
    }
    
    void loop()
    {
    
      double potansiyometre = analogRead(A0);
      if(potansiyometre <= 333)
      {
        digitalWrite(kirmizi,HIGH);
        digitalWrite(mavi,LOW);
        digitalWrite(yesil,LOW);
        
      }else if(potansiyometre > 333  && potansiyometre<=680){
      
        digitalWrite(kirmizi,LOW);
        digitalWrite(mavi,HIGH);
        digitalWrite(yesil,LOW);
      }else{
        
        digitalWrite(kirmizi,LOW);
        digitalWrite(mavi,LOW);
        digitalWrite(yesil,HIGH);
      
      }
      
      
}
