Subject: README.md

# 🛣️ Pothole Detection in Urban Roads using YOLOv8


## 🔍 Project Overview

This project focuses on detecting potholes on urban roads using **YOLOv8**.
A custom model was trained on a pothole segmentation dataset from Roboflow and tested on real road images.

---

## 📂 Dataset

* Source: Roboflow – Pothole Segmentation YOLOv8
* Format: YOLOv8 Detection
* Classes: `pothole`
* Split:

  * Train
  * Validation

---

## 🧠 Model Used

* YOLOv8 Nano (`yolov8n.pt`)
* Trained for **30 epochs**
* Image size: **640**
* Framework: **Ultralytics YOLOv8**

---

## ⚙️ Installation

```bash
python -m venv venv
venv\Scripts\activate   # Windows
pip install ultralytics
```

---

## 🚀 Training Command

```bash
yolo detect train model=yolov8n.pt data=data.yaml epochs=30 imgsz=640
```

---

## 🧪 Testing the Model

### Test on image

```bash
 yolo detect predict model=runs/detect/train4/weights/best.pt source=test_images
```

---

## 📊 Results

Sample detection results are available in the **predict/** folder.


