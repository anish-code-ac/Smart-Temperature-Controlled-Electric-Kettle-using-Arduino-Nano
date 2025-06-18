
# 🔌 Smart Temperature-Controlled Electric Kettle

This project transforms a standard electric kettle into a **smart, user-programmable kettle** using an Arduino Nano. By setting a custom temperature range (40°C to 100°C), users can boil water to a precise level for tea, coffee, or other needs.

---

## 📸 Project Preview

<img src="circuit_diagram.png" alt="Circuit Diagram" width="600"/>

---

## 🚀 Features

- 🎛️ Rotary Encoder: Set target temperature with precision
- 🌡️ DS18B20 Temperature Sensor: Accurate digital temperature readings
- 🖥️ OLED Display: Live temperature display and UI
- ⚡ Relay Module: Controls the AC-powered kettle safely
- 🔔 Optional Buzzer: Beeps when target temperature is reached
- 🔒 Safe Design: Separation of high- and low-voltage circuits

---

## 🧰 Components Used

| Component              | Description                         |
|------------------------|-------------------------------------|
| Arduino Nano           | Microcontroller board               |
| DS18B20                | Waterproof digital temperature sensor |
| OLED Display (SSD1306) | 0.96" I2C-based display             |
| Rotary Encoder (KY-040)| For setting target temperature      |
| Relay Module (5V)      | Controls AC power to the kettle     |
| Buzzer (optional)      | Alerts when heating is done         |
| Electric Kettle        | Modified for relay-based switching  |
| 4.7kΩ Resistor         | Pull-up for DS18B20 data line       |

---

## ⚙️ How It Works

1. Rotate the encoder to set the desired water temperature.
2. The OLED displays the current and target temperatures.
3. Arduino reads the temperature using the DS18B20 sensor.
4. If the current temperature is below the target, the relay turns on the kettle.
5. When the target is reached, the relay shuts off, and the buzzer sounds (optional).

---

## 🛡️ Safety Instructions

⚠️ **Caution:** This project involves **high-voltage (AC) wiring**. Only proceed if you're experienced with electrical safety or are supervised by someone who is.

- Always unplug the kettle before modifying.
- Enclose all AC connections in an insulated box.
- Ensure solid insulation and strain relief on wires.
- Use fuses or circuit breakers for added protection.

---

## 📂 File Structure

```
├── SmartKettle.ino            # Arduino source code
├── circuit_diagram.png        # Visual schematic
├── README.md                  # This file
```

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

- [Adafruit SSD1306 OLED Library](https://github.com/adafruit/Adafruit_SSD1306)
- [DallasTemperature Library](https://github.com/milesburton/Arduino-Temperature-Control-Library)
- Inspiration from the maker and Arduino community

---
