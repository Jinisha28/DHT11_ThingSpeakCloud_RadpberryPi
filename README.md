#DHT11_ThingSpeakCloud_RadpberryPi

The Raspberry Pi is a credit-card sized computer capable of doing everything we’d expect a desktop computer to do. Raspberry Pi foundation officially provides Debian based Raspbian OS. SD card is used to store the OS. Raspberry Pi is more than computer as it provides access to the on-chip hardware i.e. GPIOs for developing an application. By accessing GPIO we can connect devices like LED, motors, sensors, etc and can control them too. 
First download Raspberry Pi OS in SD card and then install it in the desktop.
The DHT11 is a basic, ultra-low-cost digital temperature and humidity sensor. It uses a capacitive humidity sensor and a thermistor to measure the surrounding air and spits out a digital signal on the data pin (no analog input pins needed). The device only requires three connections to the Raspberry Pi. +3.3V, ground and one GPIO pin. 
In this Adafruit DHT11 library should be installed.
For interfacing DHT11 with Raspberry Pi VCC and GND of both are connected and the OUT pin is connected to one of the GPIO pins. 
ThingSpeak is an IoT analytics platform service that allows to aggregate, visualize, and analyze live data streams in the cloud.
Here ThingSpeak Cloud is used to store temperature and humidity data on the cloud server.
Here Raspberry Pi will read its CPU temperature and send it to ThingSpeak and it can be monitored anywhere in the world using the internet.
Raspberry Pi data logger should be built on ThingSpeak Cloud. To build, first open the site of thingspeak cloud and sign in and create an account and then go to my channels and create a new one. Name it and in field 1 and 2 write temperature and humidity respectively and save the channel.
The data is sent through API requests which can be found in API keys. Every channel has unique API keys and URLs. In program code this URL is used to get requests.
Write Code on python3 IDE od RPI OS.
