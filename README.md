# Real Time Arduino Weather Station with AQI
A simple and effective real-time weather and air quality monitoring station built using an Arduino NANO. This project uses a DHT11 sensor to measure temperature and humidity, and an MQ135 gas sensor to estimate the Air Quality Index (AQI). All data is displayed on a TFT screen and refreshed automatically every 5 seconds, with a visual countdown timer indicating the time until the next update.
Features
Real-time Data: Measures and displays current temperature (°C) and humidity (%).
Air Quality Monitoring: Senses various gases using the MQ135 sensor to provide an Air Quality Index (AQI) reading.
Visual Display: Presents all information clearly on a color TFT display.
Auto-Refresh: Automatically updates sensor readings every 5 seconds.
Update Countdown: Shows a countdown timer on the screen, so you know exactly when the next reading will occur.
Hardware Components
Component	Description
Arduino NANO	The microcontroller brain of the project.
1.8" TFT Display	A color display to show the data.
DHT11 Sensor	Measures temperature and humidity.
MQ135 Sensor	Gas sensor used for monitoring air quality.
Breadboard	To assemble the circuit without soldering.
Jumper Wires	For making connections between components.
Software & Libraries
This project is built using the Arduino IDE. You will need to install the following libraries through the Arduino IDE's Library Manager (Tools > Manage Libraries...):
Adafruit GFX Library: The core graphics library.
Search for Adafruit GFX Library in the Library Manager.
Adafruit ST7735 and ST7789 Library: Driver for the TFT display.
Search for Adafruit ST7735 in the Library Manager. (Note: If you have a different display like an ILI9341, install the corresponding Adafruit library).
DHT sensor library by Adafruit: For interfacing with the DHT11 sensor.
Search for DHT sensor library in the Library Manager.
MQ135 Library: A library to simplify reading values from the MQ135 sensor. A popular choice is the one by G.K.Das.
Search for MQ135 in the Library Manager.
Wiring & Circuit Diagram
Connect the components to the Arduino NANO as described in the table below.
Power Connections:
Connect the VCC/5V pin of all sensors and the display to the 5V pin on the Arduino.
Connect the GND pin of all sensors and the display to a GND pin on the Arduino.
Data Connections:
Component Pin	Arduino NANO Pin
TFT       VCC     	5V
TFT       GND	      GND
TFT       CS	      D10
TFT       RESET	    D8
TFT       DC/A0	    D9
TFT      SDA/MOSI	  D11
TFT      SCK	      D13
TFT      LED	      3.3V or 5V
DHT11    Data     	D2
MQ135    A0	        A0
