# Hardware-Wireless-Main-Server


<h2>Keynotes</h2>

- Creates local Access Point and starts server there, where user can enter his GreenHouse account credentials and his WiFi network SSID and password.
- When SSID abd password for wifi network accuired, connects to the network and establishes connection with remote server.
- Telemetry from all sensors is sent to this module, anfter processing which, the needed subsystems such as heaters, light level, sprinklers etc. which are connected to relay are regulated accordingly. After that, sensor data is sent to the server, and a check for a new climate config on server is made and if so, is being downloaded.
- All manipulations are made either through a local page on a web server, a change of data on remote server or touch screen, installed on this Hardware main server.



<h2>Setup</h2> 

To setup a device, clone a repo and compile upload a code to a ESP32 with programmator or ide such as ArduinoIDE/PlatformIO
<h3>Used side libraries:</h3> 

- ESPAsyncWebServer: https://github.com/me-no-dev/ESPAsyncWebServer

- TFT_eSPI by Bodmer: https://github.com/Bodmer/TFT_eSPI

- ESP-32 core for arduino: https://github.com/espressif/arduino-esp32