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

Our project was developed in a Python environment. You can set up the required dependencies by running the following command:

  ```bash
!pip install ultralytics
  ```
This command will install the ultralytics library, which includes all the necessary components for running the YOLOv8 model, including torch, pandas, and matplotlib.
  
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
from ultralytics import YOLO

!yolo train data="yolo_params.yaml" model="yolov8l.pt" epochs=100 imgsz=640
```
- yolo_params.yaml: Contains dataset path and class definitions.

- yolov8l.pt: Pre-trained YOLOv8 large model.

- epochs=500: Training duration.

---

## 🧪 Inference
To run inference using our final, trained model (best.pt), use this simple command:

```bash
!yolo predict model="runs/detect/train/weights/best.pt" source="test_image.png" conf=0.1
```

- Results will be saved as new images with bounding boxes in the runs/ directory

---

## 📂 Project Structure
```bash
├── yolo_params.yaml       # Dataset config file
├── train.py               # Training script
├── predict.py             # Inference script
├── runs/                  # Model weights & logs
├── NeuraNova_Report.pdf   # Detailed methodology & results
└── README.md              # This file
```

---

## 👥 Team Members
- Mohit Jain (Team Leader)
- Madhu Pilli

---

## 💬 Acknowledgments
Thank you to Duality AI for hosting this hackathon and providing an innovative platform and dataset. We look forward to your feedback and the opportunity to contribute to space-tech innovation! 🛸

---

## 📧 Contact
Feel free to reach out via GitHub or email for any questions or collaborations!

---

## 🙋‍♂️ Author

Built with ❤️ by Team NeuraNova

Feel free to connect or collaborate!

- 🔗 [LinkedIn](https://www.linkedin.com/in/mohit-jain-dev/)  
- 💻 [GitHub](https://github.com/Mohitjain9654)  
- 🌐 [Portfolio Website](https://mohitjain-portfolio.vercel.app/)  
- 📧 Email: mohitjain965405@gmail.com, 418214brigadiermadhu@gmail.com

---
