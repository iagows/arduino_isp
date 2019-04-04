# ArduinoISP2 #

 March 2012 William Phelps - wm (at) usa.net 
 
 This is a fork of Adafruit's ArduinoISP
 which is a fork of Arduino's ArduinoISP
 which adds an 8 MHZ 'crystal' output on pin #9 so you don't need an
 extra oscillator/crystal. Can also rescue some bricked chips with
 bad oscillator fuses
 
**Modified for Arduino IDE 1.0**  
 shorter serial port receive buffer requires changes  
 getEOP() now gets entire request before avrisp() is called to process it  
 Serial.print((char) xxx) changed to Serial.write(xxx)  
 uint8_t changed to byte  
 added support for Piezo speaker  
 moved Pmode LED to A0  
 removed "heartbeat" on pin 6, added short blip of ERROR LED instead  
 Why is it that PROG_FLASH and PROG_DATA don't actually do anything???  
 Tested with Arduino IDE 22 and 1.0  
 IDE 22 - 5148 bytes  
 IDE 1.0 - 5524 bytes!  