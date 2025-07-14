# 🧠 Object Detection and Comparison

A computer vision project leveraging YOLOv5 for object detection on video frames and model evaluation.  
This project was created as part of the Phase 2 assignment for the Computer Vision Engineer role at **TECH AT PLAY**.

---

## 📌 Overview

This repository contains solutions for the following tasks:

### ✅ Task 1: Detection Summary Engine
- Object detection on every 5th frame of a short video using YOLOv5.
- Outputs:
  - Per-frame detection results (`.json`)
  - Total objects per class
  - Most diverse frame by object class
  - Bar chart of object frequency
  - Optional: annotated frames

### ✅ Task 3: Model Comparison and Deployment
- Evaluation of **YOLOv5n** vs **YOLOv5s** using the same 10 images.
- Metrics compared:
  - Average inference time
  - Total detections
  - Class diversity
- Outputs:
  - Tabulated results
  - Inference outputs
- Deployment:
  - Dockerfile to automate model inference from input folder to output folder

---

## 📁 Folder Structure

ObjectDetection-and-Comparison/
├── Task1_DetectionSummary/
│   ├── task1.ipynb
│   ├── task1.pdf
│   ├── detection_results.json
│   ├── object_frequency_chart.png
│   └── README.md
│
├── Task3_ModelComparison/
│   ├── task3.ipynb
│   ├── task3.html  (or task3.pdf)
│   ├── Dockerfile
│   ├── images/
│   ├── outputs/
│   └── README.md
│
└── README.md  ← main project-level README


---

## 🐳 Docker Instructions (Task 3)

### ▶️ Build Docker Image
```bash
docker build -t yolov5-inference .

▶️ Run Inference

docker run --rm -v "$(pwd)/images:/app/images" -v "$(pwd)/outputs:/app/outputs" yolov5-inference

Replace $(pwd) with full path if on Windows (e.g., C:/Users/Gaurav/...)

Results will be saved in the outputs/ folder



---

🔧 Technologies Used

Python

OpenCV

YOLOv5 (Ultralytics)

Jupyter Notebook

Matplotlib, JSON, Pandas

Docker



---

🧑‍💼 Author

Gaurav Jha
GitHub: @GauravGit-007
Email: 007gouravjha@gmail.com


---

📎 License

This project is submitted as part of a technical assessment and is intended for educational review only.

