# 🚗 P-Vision: AI-Driven Pedestrian Detection & Collision Warning

**P-Vision** is an AI-powered Advanced Driver Assistance System (ADAS) designed to improve road safety. Using the YOLOv8 object detection model, it identifies pedestrians and vehicles in real time, predicts movement patterns, and alerts drivers to potential collision risks.

## 🔍 Key Features
- Real-time pedestrian and vehicle detection using YOLOv8
- Collision risk prediction and driver alerting
- Custom training support for 9 annotated object classes

## 🧠 Dataset
The system is trained on a custom dataset containing the following 9 classes:
`Car`, `Pedestrian`, `Van`, `Cyclist`, `Truck`, `Misc`, `Tram`, `Person_sitting`, `DontCare`

### 📊 Dataset Distribution and Annotations
![Dataset Analysis](./30aae1ce-799e-4991-a494-04882182dc94.jpg)

This plot shows class distribution, bounding box sizes, and spatial position density. It highlights a class imbalance, with significantly more `Car` and `Person_sitting` instances.

## 📈 Model Evaluation
![Confusion Matrix](./2c68fd24-443c-4be6-8020-6aaadfbf075d.png)

The confusion matrix shows strong detection performance for common classes like `Car`, but reveals misclassifications between similar classes such as `Pedestrian`, `Van`, and `Cyclist`.

## 📁 Project Structure
- `data.yaml` — Dataset configuration
- `*.ipynb` — Jupyter notebooks for training and evaluation
- `yolov8n.pt` — Pre-trained YOLOv8 weights

## 🛠 Requirements
- Python 3.8+
- Install dependencies with:
  ```bash
  pip install ultralytics opencv-python numpy
