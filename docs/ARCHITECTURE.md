# Architecture

1. A Python script captures an image from a webcam.
2. YOLOv5 runs inference and writes detections to JSON.
3. A Flask API serves the latest detection results.
4. The ESP8266 polls the `/data` endpoint.
5. If a target object is detected with sufficient confidence, the ESP8266 triggers an action.

## Main folders

- `backend/python/`: vision + Flask API scripts
- `firmware/esp8266_client/`: ESP8266 polling client
- `media/screenshots/`: UI and demo screenshots
- `examples/`: sample JSON outputs
