# 🚀 NeuraNova - Duality AI Space Station Hackathon Submission

Welcome to the official repository for **NeuraNova**'s submission to the **Duality AI Space Station Hackathon**. Our project focuses on developing and optimizing a high-performance object detection model using the **YOLOv8** framework to identify key objects aboard a synthetic space station environment.

---

## 🛰️ Project Overview

This project involves:
- Training an object detection model to identify **Toolbox**, **Oxygen Tank**, and **Fire Extinguisher**.
- Utilizing **synthetic datasets** from **Duality AI's Falcon platform**.
- Applying advanced techniques in YOLOv8 to maximize accuracy and minimize false detections.

---

## 📊 Final Performance Metrics

| Metric        | Score         |
|---------------|---------------|
| **mAP@0.5**    | [Your Final mAP Score]% |
| **Precision**  | [Your Precision Score]% |
| **Recall**     | [Your Recall Score]% |

---

## 🔁 How to Reproduce Our Final Results

### 1. ✅ Environment Setup

Install dependencies using the provided script:

- **Mac/Linux**:  
  ```bash
  setup_env.sh
  ```
- **Windows:
    ```bash
    setup_env.bat
    ```
---
## Required Dependencies:
- ultralytics
  
---
## 2. 📁 Dataset
- Use the dataset provided by Duality AI.

- Structure should follow:
```bash
dataset/
  ├── train/
  ├── val/
  └── test/
```
- Ensure paths are correctly specified in yolo_params.yaml.

---

## 3. 🏋️ Model Training
Train the model from scratch using:

```bash 
yolo train data="yolo_params.yaml" model="yolov8l.pt" epochs=100 imgsz=640
```
- yolo_params.yaml: Contains dataset path and class definitions.

- yolov8l.pt: Pre-trained YOLOv8 large model.

- epochs=500: Training duration.

---
