# Real-Time Gas & Smoke Detection and Air Quality Prediction Using ML

An IoT-based smart monitoring system that detects gas leaks and smoke in real-time while predicting air quality using machine learning models. The system enhances safety by providing early alerts and intelligent environmental insights.

---

## Features

* Real-time gas and smoke detection
* Temperature and humidity monitoring
* Machine Learning-based air quality prediction
* Alert system for hazardous conditions
* Cloud integration for remote monitoring
* Data visualization dashboard (optional)
* IoT-enabled system using ESP32

---

## Tech Stack

### Hardware

* ESP32 / Arduino
* MQ Gas Sensor (MQ-2 / MQ-135)
* Temperature & Humidity Sensor (DHT22)
* Buzzer / LED

### Software

* Embedded C / Arduino IDE
* Python (ML model)
* Node.js
* React.js

### Machine Learning

* LSTM → Long Short-Term Memory
  (A type of recurrent neural network used for time-series prediction and sequence data)
* ARIMA → AutoRegressive Integrated Moving Average
  (A statistical model used for time-series forecasting)

### Cloud

* MongoDB 

---

## Working Principle

1. Sensors collect environmental data:

   * Gas concentration (MQ sensor)
   * Temperature & humidity (DHT sensor)

2. ESP32 processes the data:

   * Detects abnormal gas/smoke levels
   * Sends data to cloud

3. Machine Learning model:

   * Trained on environmental datasets
   * Predicts air quality (Good / Moderate / Hazardous)

4. Alerts are triggered when:

   * Gas/smoke exceeds threshold
   * Poor air quality is predicted

---

## Installation & Setup

### 1. Hardware Setup

* Connect MQ sensor to analog pin
* Connect DHT sensor to digital pin
* Connect buzzer/LED
* Power the ESP32

---

### 2. Firmware Setup

```bash
# Open Arduino IDE
# Select ESP32 board
# Upload code from firmware folder
```

---

### 3. Configure Wi-Fi

```cpp
const char* ssid = "YOUR_WIFI_NAME";
const char* password = "YOUR_WIFI_PASSWORD";
```

---

### 4. ML Model Setup

```bash
cd ml-model
pip install -r requirements.txt
python train_model.py
```

---

### 5. Run the System

* Power ON device
* Monitor data via Serial Monitor
* Check cloud dashboard
* Observe ML predictions

---

## Output

* Gas/smoke levels
* Temperature and humidity readings
* Air quality prediction (Good / Moderate / Poor)
* Alerts for dangerous conditions

---

## Machine Learning Details

* Input Features:

  * Gas concentration
  * Temperature
  * Humidity

* Output:

  * Air Quality Index

* Models Used:

  * LSTM → Long Short-Term Memory
  (A type of recurrent neural network used for time-series prediction and sequence data)
  * ARIMA → AutoRegressive Integrated Moving Average
  (A statistical model used for time-series forecasting)

---

## Alert System

* Buzzer activates on high gas levels
* LED indication for warning
* Mobile notifications

---

## Future Enhancements

* Mobile app integration
* Advanced cloud analytics
* Deep learning models
* Industrial deployment
* Real-time notification system

---

## Limitations

* Sensor calibration required
* Environmental factors may affect readings
* ML accuracy depends on dataset quality

--
