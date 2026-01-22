# Lab1
# LAB1: Temperature Sensor with Relay Control (Telegram)

---

## Task 1: Sensor Read & Print
The ESP32 reads temperature and humidity data from the DHT22 sensor every 5 seconds.  
The values are displayed in the serial monitor with two decimal places.

📷 *Serial monitor screenshot will be added here*

---

## Task 2: Telegram Send
The ESP32 sends a test message to Telegram using the Telegram Bot API.  
This confirms that Wi-Fi and Telegram communication are working correctly.

📷 *Telegram message screenshot will be added here*

---

## Task 3: Bot Commands
Telegram bot commands are implemented to control and monitor the system:
- `/status` returns current temperature, humidity, and relay state
- `/on` turns the relay ON
- `/off` turns the relay OFF

📷 *Telegram chat screenshots will be added here*

---

## Task 4: Temperature Alert Logic
- No messages are sent when temperature is below 30°C  
- When temperature is 30°C or higher and the relay is OFF, alert messages are sent every 5 seconds  
- After the `/on` command is received, alert messages stop  
- When temperature drops below 30°C, the relay turns OFF automatically and a one-time auto-OFF message is sent

🎥 *Short demo video will be added here*

---

## Task 5: Robustness
The system is designed to be robust:
- Automatically reconnects to Wi-Fi if the connection is lost  
- Handles Telegram HTTP errors without crashing  
- Skips sensor read cycle if a DHT sensor error occurs  

---

## Task 6: Documentation
This repository includes:
- MicroPython source code files  
- `README.md` with system description and usage instructions  
- Wiring diagram and Telegram screenshots  
- Demo video link  

📷 *Wiring diagram and flowchart will be added here*

---

## Author
Name: ____________________  
Lab: LAB1 – Temperature Sensor with Relay Control
