**#RoadSafe: AI-Powered Smart Traffic Monitoring and Control**
Overview:
"RoadSafe" is an intelligent traffic monitoring system designed to enhance road safety by integrating AI, IoT, and smart traffic control. The system leverages AI-powered traffic cameras and smart traffic lights to detect red-light violations, accidents, and real-time traffic conditions, ensuring safer and more efficient roads.

Key Features:

✅ AI-Based Traffic Monitoring – Detects red-light violations, captures license plates using OCR (Optical Character Recognition), and automatically issues alerts for traffic infractions.
✅ Real-Time Accident Detection – Identifies collisions at intersections and instantly notifies traffic authorities for swift emergency response.
✅ Smart Traffic Light System – A crossroad traffic control system built with an Arduino Mega and ESP8266, featuring:

Four traffic lights operating on a fixed sequence (Red: 9s, Yellow: 3s, Green: 9s).

Dynamic LED brightness adjustment via an LDR sensor using PWM for optimal visibility in different lighting conditions.

Manual override via a web interface for emergency situations, allowing immediate light changes when required.

How It Works:

Automated Traffic Control – The traffic lights follow a structured cycle while adapting to ambient light conditions.

Manual Signal Override – Operators can control signals remotely via a web interface to prioritize emergency vehicles.

AI-Powered Violation Detection – A simulated traffic monitoring system using a webcam detects vehicles crossing on a red light and extracts their license plate information for enforcement actions.

Backup Web Interface:
Due to WiFi restrictions preventing port forwarding, the app currently cannot access the ESP8266 remotely. However, to demonstrate feasibility, the system includes a local web interface for real-time control and monitoring. This ensures the core functionality remains operational while alternative solutions for remote access are explored.

Impact:
By integrating AI-driven monitoring with IoT-based traffic control, RoadSafe aims to:
🚦 Reduce traffic violations through automated enforcement.
🚑 Enhance emergency response with real-time alerts.
🔄 Improve traffic flow efficiency with adaptive signal control.
🌍 Ensure safer roads for all drivers and pedestrians.

This project showcases a scalable, AI-enhanced traffic management system, bridging smart city innovations with real-world safety solutions.
