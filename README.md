# Kruk
A small car computer with a temperature sensor, stopwatch and free Wi-Fi for all your friends.


<video>src="https://github.com/SabasSolutions/Kruk/raw/refs/heads/main/video/kruk.mp4" controls style="max-width:100%;"></video>
![video](https://github.com/SabasSolutions/Kruk/raw/refs/heads/main/video/kruk.mp4)
[Video on YouTube](https://youtube.com/shorts/VVHMmDFvbYU)

###Components needed for assembly:
1. ESP32C3 (WeActStudio ESP32-C3FH4)
2. WeActStudio DC/DC DCM1 5V
3. SSD1306 4 pin display
4. DS18B20 Temperature Sensor
5. Resistor 4.7K
6. Wires 30AWG

###Connecting the wires to board:
**SSD 1306**
SDA -> 8
SCL -> 9
VCC -> 3V3
GND -> G

**DS18B20**
RED -> 3V3
BLACK -> G
YELLOW -> 10

**Power Supply**
We connect power from the car via the WeActStudio DC/DC DCM1 5V module.
Then
+ -> 5V
- -> G




