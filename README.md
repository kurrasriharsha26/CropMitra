# 🌱 CropMitra – Smart Irrigation System Using IoT

**CropMitra** is an innovative IoT-enabled smart irrigation system that empowers farmers to optimize water usage, automate irrigation, and improve crop yield using real-time data from soil and weather sensors.

---

## 📘 Project Overview

CropMitra leverages the power of **IoT**, **sensors**, and **automation** to monitor soil moisture and weather conditions, helping farmers make data-driven decisions for irrigation. It ensures **efficient water management**, **cost savings**, and promotes **sustainable agriculture**.

The system uses sensors connected to a **NodeMCU ESP8266** microcontroller to collect soil moisture and temperature data. Based on these readings, it automatically controls a water pump through a relay module. A web-based interface (built using **HTML, CSS, and JavaScript**) displays real-time data and allows remote monitoring.

---

## 🧠 Key Features

- 🌾 **Automated Irrigation** – Water pump activates automatically based on soil moisture readings.  
- ☁️ **Weather-Adaptive Scheduling** – Delays watering if rainfall or high humidity is detected.  
- 📶 **IoT Integration** – Real-time communication via ESP8266 Wi-Fi module.  
- 📊 **Web Dashboard** – Displays live soil and environmental data with visual charts.  
- 🔔 **Alerts & Notifications** – Provides irrigation alerts and moisture level updates.  
- ⚙️ **Customizable Thresholds** – Configurable moisture and temperature limits.  
- 🌍 **Eco-Friendly** – Reduces water wastage and supports sustainable farming.  

---

## 🧩 System Architecture

### **Hardware Components**
- NodeMCU ESP8266 (Microcontroller)
- Soil Moisture Sensor
- DHT11 Sensor (Temperature & Humidity)
- Relay Module
- DC Water Pump
- Jumper Wires
- Breadboard
- Power Supply (Battery/Solar)

### **Software Tools**
- Arduino IDE (for programming NodeMCU)
- HTML, CSS, JavaScript (for web interface)
- Figma (for UI design prototype)

---

## ⚙️ Working Principle

1. The **soil moisture sensor** reads real-time soil humidity levels.  
2. The **ESP8266** processes sensor input and decides whether irrigation is required.  
3. If soil is dry, the **relay module** triggers the **water pump**.  
4. When the optimal moisture level is achieved, the pump is automatically turned off.  
5. The **DHT11 sensor** monitors temperature and humidity to adjust irrigation logic.  
6. Data is sent to the **web dashboard** for real-time monitoring.

---

## 🌐 Web Application Overview

The CropMitra web app offers three main pages:

- **Login/Signup Page** – Secure authentication for users.  
- **Dashboard** – Displays real-time soil moisture, temperature, and pump status.  
- **Summary Page** – Shows ideal conditions for various crops.  

All data updates dynamically using JavaScript to ensure a smooth user experience.

---

## 🧠 Methodology

1. Assemble hardware components (ESP8266, sensors, relay, pump).  
2. Write and upload Arduino code using **Arduino IDE**.  
3. Develop and deploy a responsive web interface using HTML, CSS, and JavaScript.  
4. Connect ESP8266 to Wi-Fi to enable real-time updates.  
5. Test the system under different soil and weather conditions.

---

## 💻 Implementation Code Snippet

Example of the main logic for sensor reading and relay control:

```cpp
if (moisture > MOISTURE_THRESHOLD_DRY) {
    digitalWrite(RELAY_PIN, HIGH); // Turn pump ON
    Serial.println("Soil is dry – activating irrigation");
} else {
    digitalWrite(RELAY_PIN, LOW);  // Turn pump OFF
    Serial.println("Soil moisture is optimal – irrigation stopped");
}

🧾 Conclusion

CropMitra provides a cost-effective, sustainable, and scalable solution for modern farming. By combining IoT and automation, it optimizes water use, enhances crop yield, and supports environmental conservation.
This project represents a step toward smart agriculture and sustainable resource management.

👨‍💻 Team Members
Name	Roll No.
K. Sri Harsha	24R05A0524
M. Navya	24R05A0527
M. Lokesh	24R05A0530
P. Navyasri	24R05A0535

🎓 Institution

CMR Institute of Technology (UGC Autonomous)
Approved by AICTE | Affiliated to JNTUH | Accredited by NBA and NAAC
Kandlakoya (V), Medchal District – 501401
www.cmrithyderabad.edu.in

🔗 References

IEEE Paper on IoT Smart Irrigation

ResearchGate: IoT Smart Irrigation System for Precision Agriculture

MDPI – Smart Agriculture Sensors

IOP Science – Smart Irrigation Architecture

🛠️ Future Enhancements

Integration with mobile app notifications.
Use of solar power for complete energy independence.
Integration with machine learning models for predictive irrigation.
Adding database and analytics dashboards for long-term farm insights.
ALSO finding a which type of disease and solution for the crops. 

