# ✈️ Airport Anomaly Detection System using YOLOv8 & Augmented Reality

A real-time anomaly detection and alert system for airport environments. This project uses custom-trained **YOLOv8** models to detect **weapons**, **suspicious behavior**, and **threats**, leveraging **multi-camera surveillance** and **augmented reality (AR)** overlays to enhance situational awareness and security response.

---

## 📌 Features

- 🔪 Detects **weapons** (e.g., knives, firearms) using YOLOv8  
- 🚨 Identifies **aggressive or abnormal behavior** in public zones  
- 🎥 Supports **multiple surveillance cameras**  
- 🧠 Uses **AR overlays** for intuitive visualization  
- 📡 Sends **real-time alerts** to security personnel  
- 🧰 Modular and scalable for large infrastructures  

---

## 🧠 Technologies Used

- [YOLOv8 (Ultralytics)](https://github.com/ultralytics/ultralytics)  
- Python (OpenCV, NumPy, PyTorch)  
- Augmented Reality toolkit (e.g., OpenCV AR markers or Unity integration)  
- WebSockets / MQTT for real-time alert communication  
- Optional: Flask or FastAPI for backend services  

---

## 🏗️ Project Structure

\`\`\`bash
├── datasets/          # Custom training datasets (weapons, behaviors)
├── models/            # Trained YOLOv8 models
├── src/               # Main detection and AR logic
│   ├── detection.py
│   ├── ar_overlay.py
│   ├── camera_handler.py
│   └── alert_system.py
├── configs/           # Configuration files
├── requirements.txt
└── README.md
\`\`\`

---

## 🚀 Getting Started

### 1. Clone the repository

bash
git clone https://github.com/your-username/airport-anomaly-detection.git
cd airport-anomaly-detection

### 2. Set up the environment

\`\`\`bash
pip install -r requirements.txt
\`\`\`

### 3. Download or train the YOLOv8 model

You can train your custom YOLOv8 model on your labeled dataset or use a pre-trained one.

\`\`\`bash
# Example training command (using Ultralytics CLI)
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50 imgsz=640
\`\`\`

### 4. Run the system

\`\`\`bash
python src/detection.py
\`\`\`

---

## 📊 Example Use Cases

- Airport terminals and gates  
- Luggage and security checkpoints  
- Real-time suspicious behavior monitoring in waiting areas  

---

## 📎 Future Enhancements

- Integration with facial recognition for suspect identification  
- Voice alerts and speaker output  
- Centralized dashboard for all camera feeds and alerts  
- Mobile AR support for on-the-ground security staff  

---

## 🙏 Acknowledgments

- [Ultralytics](https://github.com/ultralytics/ultralytics) for YOLOv8  
- OpenCV for AR and computer vision  
- Airport security datasets from Kaggle and custom labeling  

---

## 📜 License

This project is licensed under the **MIT License**.
EOF
