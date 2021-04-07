# Examensarbete


Konfiguera blynk APP - Vid skapande av egen blynk server (https://github.com/blynkkk/blynk-server)

#define BLYNK_PRINT Serial

#include <Adafruit_BMP280.h>
#include <Adafruit_Sensor.h>
#include <Wire.h>
#include <ESP8266_Lib.h>
#include <BlynkSimpleShieldEsp8266.h>
#include <DHT.h>

char auth[] = "Auth koden från Blynk Appen!";


char ssid[] = "";
char pass[] = "";


#define EspSerial Serial3

#define ESP8266_BAUD 115200

ESP8266 wifi(&EspSerial);

#define DHTPIN 4      
//  pin koppling.

#define DHTTYPE AM2302   


DHT dht(DHTPIN, DHTTYPE);
Adafruit_BMP280 bmp;//creating object for bmp280
BlynkTimer timer_dht
BlynkTimer timer_bmp;
BlynkTimer timer_mq2;



const int calibrationLed = ;
                      
const int MQ_PIN = ;     
                         
const int MQ_power = ;

int RL_VALUE = ; 
                                  
float RO_CLEAN_AIR_FACTOR = ;
                   
#define MQ_powerPin 8
