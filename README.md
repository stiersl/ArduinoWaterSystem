# ArduinoWaterSystem
ArduinoWaterSystem with WebServer
 
 This sketch is written for an Arduino Mega2560 with an ethernet shield W5100. 
 This arduino will  control 5 solenoid values which control the water to five different
 watering zones(connected to PINS 5-9) There is a flow meter connected to PIN 3
 which is used to measure the flow rate of the water to any of the zones.

 This program will also accept HTTP requests to both open and close the values and it 
 will also return the state of the valves and flowmeter in the body of the returned. The 
 body is returned in the form of a JSON.

 As a safety measure when 3 gallons of water have been measured in any zone that zone is
 automatically closed to limit the amount of water used.
 
 S.Stier 4/29/2020  V0.0.2
