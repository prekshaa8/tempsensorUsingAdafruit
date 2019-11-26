# Temperature-monitoring-using-Adafruit-IoT-Platform:

This temperature monitoring system is based on Adafruit cloud service, ESP8266 microcontroller (MCU) and Message Queuing Telemetry Transport (MQTT) protocol. Adafruit IoT Platform is the user-friendly cloud service with GUI Dashboard and contains a vast catalogue of certified IoT-ready devices and connectivity options. This allows users to easily add any device to the library utilising MQTT API. All devices in Adafruit are interoperable and benefit from features such as asset tracking, remote monitoring and control, and tools to visualise real-time and historical data.

Required components:
ESP8266 dev module
Jumper wires
Bread Board
DHT11 temperature and humidity sensor

# Circuit Connections:
ESP8266 PIN-OUT TO TEMPERATURE SENSOR PINS
```
  A0	                    OUT
  
 3V -VCC	              VCC
 
  Gnd                      Gnd
```
# ESP8266 programming with Arduino IDE:
You need Arduino IDE software to program ESP8266. Download the latest Arduino IDE from here and install it. 

Steps for adding ESP8266 board and library to Arduino IDE are given below.

1.Open Arduino IDE.

2.Go to File menu and select Preferences.

3. Copy the below-mentioned package and paste in Additional Boards Manager URL. 
http://arduino.esp8266.com/stable/package_esp8266com_index.json

4.Go to Tools and select Boards Manager.

5.Search ESP8266 and Install the latest version.

6.From the tools menu, select NodeMCU 1.0 (ESP-12E Module) board.

7.Select Include Library from Sketch menu. And install Adafruit MQTT library, DHTesp
Or

8.Download Adafruit MQTT library from here and add the zip file by navigating to include the library in Sketch and add zip file.

9.Download DHTesp library from here and add the zip file by navigating to include the library in Sketch and add zip file
After adding all details in the code, compile it and upload the program (sketch) using a standard USB cable to ESP8266.

# Hardware interfacing with Adafruit IoT platform

Open Adafruit.IO and sign in using your account


1.Create a new Dashboard where the temperature value are viewed.

<img src="https://github.com/prekshaa8/tempsensorUsingAdafruit/blob/master/newDB.png" height="240" width="480">


2.Navigate to Feed, and in ‘actions’ block create a new Feed 


<img src="https://github.com/prekshaa8/tempsensorUsingAdafruit/blob/master/actions.png" height="240" width="480">

<img src="https://github.com/prekshaa8/tempsensorUsingAdafruit/blob/master/newFEED.png" height="240" width="480">

3.Add the feed name in the FEEDS Category ‘feed name’ of the Arduino code.


<img src="https://github.com/prekshaa8/tempsensorUsingAdafruit/blob/master/arduinoFEED.JPG" height="75" width="300">

4.Compile and Upload the code.
5.Before that make sure that WiFi is turned on.
6.To check the output, Adafruit acts as a visualizer. To check the output offline open Serial Monitor in the top right corner of the Arduino IDE
   Note: Make sure that the Baud rate is the same as the Serial. begin rate


<img src="https://github.com/prekshaa8/tempsensorUsingAdafruit/blob/master/feeds.png" height="240" width="480">

NOTE:
Temperature monitoring can also be done using other IoT platforms like Thingspeak, Cayenne, firebase, asksensors etc.

