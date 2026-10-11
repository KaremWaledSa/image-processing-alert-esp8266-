# ESP8266 Image Processing Alert

A small IoT + computer-vision demo where a Python backend performs object detection and an ESP8266 client polls the detection API and triggers an alert action.

## What this project does
- captures an image from a webcam
- runs object detection with YOLOv5
- exports detections as JSON
- exposes the latest detections through a Flask API
- lets an ESP8266 react to specific detected objects

## Tech stack
- ESP8266 / Arduino
- Python
- Flask
- OpenCV
- PyTorch / YOLOv5

## Repository structure
```text
firmware/esp8266_client/
backend/python/
media/screenshots/
examples/
docs/
```

## Why this repo is worth showing
This project is better than a basic Arduino sketch because it combines:
- embedded networking
- a lightweight backend API
- computer vision
- device-side reaction logic

## Demo assets
Add:
- 1 short video
- 2 screenshots from `media/screenshots/`
- 1 architecture image

## Next improvements
- move configuration into `.env`
- publish confidence thresholds as variables
- replace polling with MQTT or WebSocket messaging
- add a proper action endpoint on the ESP8266 side


## Security Placeholder Status

All publishable examples in this repo should use placeholders instead of real secrets:
- `YOUR_WIFI_SSID`
- `YOUR_WIFI_PASSWORD`
- `YOUR_BLYNK_TEMPLATE_ID`
- `YOUR_BLYNK_TEMPLATE_NAME`
- `YOUR_BLYNK_AUTH_TOKEN`
- `YOUR_COMPUTER_IP`
- `YOUR_DEVICE_IP`

Do not commit real Wi-Fi credentials, Blynk tokens, cloud endpoints, or machine-local IPs.
