# 🚧 Pothole Segmentation for Road Damage Assessment

This project focuses on detecting & segmenting potholes from road images using machine learning techniques. The goal is to provide an automated and accurate method for road damage assessment, improving the efficiency of maintenance operations.

## 📌 Project Highlights

- **Objective**: Detect and segment potholes in road surface images.
- **Approach**: Fine-tuned YOLOV8-seg for Pothole detection and segmentation.
- **Dataset**: Pothole Image Segmentation Dataset, RDD2022 or equivalent road surface datasets with labeled masks.
- **Libraries Used**: PyTorch, OpenCV, Albumentations, Matplotlib.

## 🧠 Model Details

- **Architecture**: YOLOv8n-seg model fine-tuned on dataset
- **Loss Function**:YOLOv8n-seg uses a loss function that combines bounding box loss (CIoU or DIoU), class loss (BCE or CCE), mask loss (Dice or BCE), and objectness loss (BCE)..
- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - Mean Average Precision at IoU(mAP50)

## 📁 Folder Structure
Pothole_Segmentation/
├── train/
│   ├── images/         # Training images 
│   └── labels/         # Training labels
├── valid/
│   ├── images/          # Validation images
│   └── labels/          # validation labels
├── data1.yaml           # Dataset configuration file
├── README.dataset.txt   # Dataset description
├── README.roboflow.txt  # Auto-generated README 
└── sample_video.mp4     # Sample video to test model


## Clone the Repository

You can clone this repository using the following command:

git clone https://github.com/SaniyaManiyar0102/Pothole detection and segmentation using YOLOV8.git

pip install -r requirements.txt
