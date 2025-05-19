# IOT-URBAN-AIR-MONITORING-
steps to run the project:

 step 1: Install the Required Librarie in the Arduino IDE:
   - `WiFi.h` (built-in for ESP32)
   - `HTTPClient.h` (built-in for ESP32)
   - `DHT sensor library` by Adafruit
   - `Adafruit Unified Sensor` library

 step 2:  Upload the source code...
   - Open the `AirQualityMonitor.ino` file in Arduino IDE
   - Replace the placeholders in the code:
     ```cpp
     const char* ssid = "Your_SSID";
     const char* password = "Your_PASSWORD";
     http.begin("http://your-server.com/update"); // you can put the appropiate details on it ...thats your wish
     ```
   - Select the correct board (`ESP32 Dev Module`) and port
   - Upload the sketch

  step 3: Connect to Serial Monitor
   - Set the baud rate to `115200`
   - You should see temperature, humidity and methane level readings
