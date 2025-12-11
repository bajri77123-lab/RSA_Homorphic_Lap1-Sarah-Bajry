What is the Project?
This project is a simulation of IoT (Internet of Things) security mechanisms.
It demonstrates how IoT devices protect their data and ensure secure communication with a server.
The project is divided into three major parts, each covering a different security concept:
1.	IoT Data Encryption Using AES-GCM
2.	IoT Device Security Lifecycle
3.	Secure Boot Verification
Part I — IoT Sensor Data Encryption Simulation
This part simulates an IoT device sending secure sensor readings (temperature & humidity) to a server.
Purpose
To demonstrate how an IoT device:
1.	Collects sensor data
2.	Encrypts it using AES-GCM (secure encryption with authentication)
3.	Sends the encrypted data to a server
4.	The server then decrypts and verifies that the data was not altered
Process Overview
1.	Generate sensor data
Temperature (20–40 °C)
Humidity (30–80%)
2.	Generate a secret AES encryption key
3.	Encrypt the data
AES-GCM provides both confidentiality and integrity
Produces: nonce, ciphertext, authentication tag
4.	Server decrypts the data using the same key
5.	If decrypted data matches the original → SUCCESS
Goal
To show how secure IoT communication works using modern cryptography.



Part II — IoT Device Lifecycle Simulation
This part simulates the five security stages of an IoT device from manufacturing to disposal.
The five stages
1.	Threat Modeling
Identify risks, threats, entry points, and mitigation strategies.
2.	Secure Boot Initialization
Ensures the device starts only if firmware is trusted.
3.	Key Injection
Securely installing cryptographic keys into the device.
4.	OTA Firmware Updates
(Over-The-Air updates) Checking and installing trusted firmware updates.
5.	Secure Decommissioning
Wiping keys and sensitive data before retiring the device.
Goal
To simulate the lifecycle of a real IoT device with security controls applied at each stage.



How Can Anyone Run This Code?
Anyone can run the project by following these steps:
1. Install Required Library
pip install pycryptodome
2. Save the Python script into a file
Example:
assignment_solution.py
3. Run the file
python assignment_solution.py
Or run each part inside Jupyter Notebook, Google Colab, or any Python IDE.

