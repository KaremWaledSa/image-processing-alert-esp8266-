# Setup

## Python backend
1. Create a virtual environment.
2. Install `backend/python/requirements.txt`.
3. Run `api_server.py`.
4. Run `image_processing.py` to capture and detect objects.

## ESP8266 client
1. Open `firmware/esp8266_client/esp8266_client.ino`.
2. Replace `YOUR_WIFI_SSID`, `YOUR_WIFI_PASSWORD`, and `YOUR_COMPUTER_IP`.
3. Install required Arduino libraries:
   - ESP8266 board package
   - ArduinoJson
   - ESP8266HTTPClient
4. Flash the firmware and monitor serial output.

## Before public release
- keep screenshots
- add a short demo video link in the main README
- never commit real Wi-Fi credentials or local IPs
