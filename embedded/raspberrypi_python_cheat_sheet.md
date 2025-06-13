# 🍓 Raspberry Pi + Python Cheat Sheet

## 🔌 GPIO
```python
import RPi.GPIO as GPIO

GPIO.setmode(GPIO.BCM)
GPIO.setup(18, GPIO.OUT)
GPIO.output(18, GPIO.HIGH)
```

## 📷 Camera
```python
from picamera2 import Picamera2
cam = Picamera2()
cam.start()
```

## 🔌 Serial
```python
import serial
ser = serial.Serial('/dev/ttyUSB0', 9600)
ser.write(b'hello')
```