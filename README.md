# Automated-Waste-Classification-and-Segregation-System
An AI-based system that uses image processing and ML to classify waste as biodegradable, non-biodegradable, or recyclable, then automatically directs it to the correct bin using servo motors for efficient and eco-friendly disposal.

---

1. Features

- Image-based waste recognition using Convolutional Neural Networks (CNN)
- Real-time classification using camera feed
- Servo/motor control for bin segregation
- Environment-friendly and easy to deploy
- Option for mobile app or web interface (optional)

---

2. Tech Stack

- Python
- OpenCV
- TensorFlow/Keras
- Raspberry Pi or Arduino (ESP32 optional)
- Servo Motors
- Pi Camera / Webcam

---

3. Project Architecture

i.  Waste image is captured using a camera

ii. Pre-trained CNN model classifies the waste type

iii.Based on the classification:
   - Biodegradable → Bin 1
   - Non-biodegradable → Bin 2
   - Recyclable → Bin 3

iv. A servo or motor system activates to open the correct bin

---

4. Installation

```bash
# Clone the repository
git clone https://github.com/your-username/waste-classification-system.git
cd waste-classification-system

# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install required packages
pip install -r requirements.txt
```

---

5. Project structure

```bash
waste-classification-system/
│
├── model/
│   └── waste_classifier.h5           # Trained ML model
│
├── dataset/
│   └── biodegradable/
│   └── non_biodegradable/
│   └── recyclable/
│
├── main.py                           # Main file to run system
├── camera.py                         # Handles camera feed
├── servo_control.py                  # Controls bin motors
├── utils.py                          # Preprocessing and utilities
├── requirements.txt
└── README.md
```

---

6. DataSet and Model

> You can use custom waste datasets or open datasets like:

   TrashNet Dataset

> Train a CNN model (e.g., using Keras with MobileNet or simple CNN)

> Save and load the .h5 model for real-time inference

---

7. How to Run

```bash
python main.py
```

---

8. Hardware Requirements

i. Raspberry Pi / Arduino / ESP32

ii. Pi Camera or USB Webcam

iii.Servo Motors (3x for 3 bins)

iv. Power Supply

v. Jumper Wires, Breadboard

---

9. Future Enhancements

- Add LCD display to show classification result

- IoT Integration to track waste analytics online

- Add voice assistant for feedback

- Solar-powered waste bin

---



