# Kruk
A small car computer with a temperature sensor, stopwatch and free Wi-Fi for all your friends.


<video>src="https://github.com/SabasSolutions/Kruk/raw/refs/heads/main/video/kruk.mp4" controls style="max-width:100%;"></video>
![video](https://github.com/SabasSolutions/Kruk/raw/refs/heads/main/video/kruk.mp4)
[Video on YouTube](https://youtube.com/shorts/VVHMmDFvbYU)

### Components needed for assembly:
1. ESP32C3 (WeActStudio ESP32-C3FH4)
2. WeActStudio DC/DC DCM1 5V
3. SSD1306 4 pin display
4. DS18B20 Temperature Sensor
5. Resistor 4.7K
6. Wires 30AWG

### Connecting the wires to board:
**SSD 1306**\
SDA -> 8\
SCL -> 9\
VCC -> 3V3\
GND -> G

**DS18B20**\
RED -> 3V3\
BLACK -> G\
YELLOW -> 10

**Power Supply**\
We connect power from the car via the WeActStudio DC/DC DCM1 5V module.\
Then\
Positive power supply wire -> 5V\
negative power supply wire -> G

### About
Kruk (Крук) means hook in Belarusian.\
The computer was developed to replace the standard BMW E36 analog clock. It shows the temperature of the cabin or any other place where you attach the temperature sensor, and also shows the time since switching on. An additional interesting function is the distribution of "Free Wi-Fi", when the user connects, it automatically transfers to the Captive Portal, which can draw any web page that can be changed in **line 20** of the code. After connecting the first user, additional information about the number of users connected to Wi-Fi and the number of users who remain connected and have not yet disconnected from it will be displayed on the display.\
By default, the code contains a joke page for Belarusian users. The version for Russian users is in the **ru** folder.\
Flash via Arduino IDE.

> [!IMPORTANT]
> AsyncTCP and ESPAsyncWebServer libraries must be installed from the ESP32Async author in Arduino IDE. Also, don't forget to install all the other libraries. It is also necessary to install the ESP32 package from Espressif Systems in the Arduino board manager.




