// C++ code
//
int ledPins[] = {2, 3, 4, 5, 6, 7};  
int leds = 6;  

void setup() {
  for (int i = 0; i < leds; i++) {
    pinMode(ledPins[i], OUTPUT);  
  }
}

void loop() {
  
  for (int i = 0; i < leds; i++) {
    digitalWrite(ledPins[i], HIGH);   
    delay(500);                       
    digitalWrite(ledPins[i], LOW);   
  }
  
   
  for (int i = leds - 1; i >= 0; i--) {
    digitalWrite(ledPins[i], HIGH);
    delay(500);
    digitalWrite(ledPins[i], LOW);
  }
}
