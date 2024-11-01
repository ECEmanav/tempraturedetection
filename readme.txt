Temperature and Humidity Detection Using DHT11 Sensor with Arduino Uno

Overview

This project interfaces a DHT11 temperature and humidity sensor with an Arduino Uno to monitor environmental conditions. The code reads temperature and humidity data from the sensor and outputs it to the serial monitor. This is helpful for basic IoT or climate monitoring applications.

Components

Arduino Uno
DHT11 Temperature and Humidity Sensor
Jumper wires
Breadboard (optional)
Setup

Circuit Connections
Connect the VCC pin of the DHT11 to the 5V pin on the Arduino Uno.
Connect the GND pin of the DHT11 to the GND pin on the Arduino Uno.
Connect the DATA pin of the DHT11 to digital pin 2 on the Arduino Uno.
Installing DHT Library
Open the Arduino IDE.
Go to Sketch > Include Library > Manage Libraries.
Search for "DHT sensor library" and install the one by Adafruit.
Uploading Code
Open the provided .ino file in the Arduino IDE.
Verify and upload the code to the Arduino Uno.
How to Run

After uploading, open the Serial Monitor (found under Tools > Serial Monitor) in the Arduino IDE.
Set the baud rate to 9600.
Every 2 seconds, you will see the temperature (in Celsius) and humidity values from the DHT11 sensor displayed on the Serial Monitor.
Expected Output

Example output on Serial Monitor:

yaml
Copy code
Humidity: 45.0 %    Temperature: 25.0 *C
Notes

The DHT11 sensor has a humidity range of 20-90% and temperature range of 0-50°C.
Data refreshes every 2 seconds in the current configuration.
If data is not displayed, ensure connections are correct and the DHT library is installed.
Troubleshooting

No output or error: Verify sensor connections, ensure DHT11 sensor is properly connected to digital pin 2.
"Failed to read from DHT sensor!" message: This indicates a communication issue. Recheck the wiring and ensure the sensor is not faulty.
