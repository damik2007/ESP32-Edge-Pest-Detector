# Project 1: ESP32-CAM On-Device Pest Detector using Edge Impulse

## Goal
To develop a low-cost, standalone IoT device capable of automatically detecting the presence of pests on agricultural yellow sticky traps using an embedded machine learning model. The initial aim was to help farmers by providing timely pest alerts.

## How it Works
1.  An ESP32-CAM captures an image of the sticky trap.
2.  A pre-trained machine learning model, running directly on the ESP32-CAM, analyzes the image.
3.  The model classifies the image as either containing a "PEST" or "NO PEST".
4.  The result is printed to the Serial Monitor.

## Technologies Used
* **Hardware:** ESP32-CAM, FTDI Programmer
* **Software:** Arduino IDE (C++), Edge Impulse (TinyML Platform)
* **Machine Learning:** Custom Image Classification Model

## Development Process & Challenges
* **Model Training:** Trained a TinyML model on the Edge Impulse platform using a dataset of 40-50 images (photos of pest pictures on yellow traps) to achieve **98% classification accuracy**.
* **Deployment:** Successfully deployed the optimized model to the ESP32-CAM.
* **Major Challenge: Resource Constraints:** While the on-device model worked accurately for detection, it consumed nearly all the available memory and processing power of the ESP32-CAM. This critical limitation prevented the integration of necessary features like Wi-Fi connectivity for sending notifications, which was part of the original goal.
* **Key Learning:** This project provided valuable hands-on experience with the capabilities and significant limitations of running AI models directly on resource-constrained microcontrollers (Edge AI / TinyML).

## Outcome
Successfully demonstrated accurate, real-time pest detection directly on the ESP32-CAM. However, due to hardware memory constraints, the project could not fulfill the complete requirement of network connectivity, leading to the development of Project 2 (Cloud AI approach).

**(Optional: Add your photo of the ESP32-CAM setup here)**
**(Optional: Add the link to your demo video for this project here)**
