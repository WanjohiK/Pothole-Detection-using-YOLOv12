# Pothole-Detection-using-YOLOv12

## Overview

This project focuses on automatic pothole detection using the YOLOv12 object detection model. The model is trained on images annotated via Roboflow, allowing it to accurately identify and locate potholes in road images.

The aim of this project is to assist in road infrastructure monitoring and maintenance by providing an efficient computer vision pipeline that can be integrated into cameras, drones, or surveillance systems.

## Key Features

🧠 YOLOv12-based Object Detection: Leverages the latest YOLO architecture for high-accuracy real-time detection.

🖼️ Roboflow Integration: Dataset annotated and exported from Roboflow in YOLO format.
link: https://universe.roboflow.com/wanjohik/potholes-detection-tkn7o/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true

🚗 Automatic Pothole Localization: Detects and draws bounding boxes around potholes.

📊 Evaluation Metrics: Includes precision, recall, and mAP evaluation.

💻 Google Colab / Local Training: Runs easily on CPU or GPU environments.

## Project Workflow

         ┌─────────────────────┐
         │   Image Collection  │
         └──────────┬──────────┘
                    │
         ┌─────────────────────┐
         │   Annotation in     │
         │     Roboflow        │
         └──────────┬──────────┘
                    │
         ┌─────────────────────┐
         │  Dataset Export     │
         │ (YOLOv12 Format)    │
         └──────────┬──────────┘
                    │
         ┌─────────────────────┐
         │  YOLOv12 Training   │
         │   (Google Colab)    │
         └──────────┬──────────┘
                    │
         ┌─────────────────────┐
         │   Model Evaluation  │
         └──────────┬──────────┘
                    │
         ┌─────────────────────┐
         │  Pothole Detection  │
         │ on Test Images/Vids │
         └─────────────────────┘

## Tech Stack

| Component           | Technology                      |
| ------------------- | ------------------------------- |
| **Language**        | Python 3.x                      |
| **Framework**       | PyTorch / Ultralytics           |
| **Model**           | YOLOv12                         |
| **Annotation Tool** | Roboflow                        |
| **Dataset Format**  | YOLO (images + labels)          |
| **Visualization**   | OpenCV, Matplotlib              |
| **Environment**     | Jupyter Notebook / Google Colab |


## Results

| Metric    | Score |
| --------- | ----- |
| Precision | 0.94  |
| Recall    | 0.91  |
| mAP@50    | 0.93  |
