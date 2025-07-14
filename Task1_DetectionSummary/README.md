# Task 1 – Detection Summary Engine

## 👤 Candidate: Gaurav Jha  
**Assignment:** Tech At Play – Phase 2  
**Folder:** Task1_DetectionSummary  
**Submission Date:** 14 July 2025

---

## 🔍 Objective

This task uses a YOLOv5 object detection model to analyze a real-world video and generate visual and structured outputs.

### Goals:
- Use a pre-trained object detection model (YOLOv5)
- Process every **5th frame** of a 10-second `.mp4` video
- Extract:
  - Class labels
  - Bounding box coordinates
  - Confidence scores
- Count total objects per class
- Identify the frame with **maximum class diversity**
- Visualize the object frequency using a **bar chart**
- *(Optional)* Save annotated frames for visual output

---

## 🗂️ Folder Structure

```

Task1\_DetectionSummary/
├── task1.ipynb                  # Jupyter Notebook with all code
├── task1.pdf                    # PDF export of the notebook
├── video.mp4                    # Input video used for detection
├── detection\_results.json       # JSON with per-frame detection results
├── object\_frequency\_chart.png   # Bar chart of object class frequencies
├── frame\_0.jpg                  # Sample annotated frame (optional)
├── frame\_5.jpg
└── README.md                    # This documentation file

````

---

## 🧪 Sample Output Details

- ✅ `detection_results.json`: Includes all detection results from every 5th frame
- ✅ `object_frequency_chart.png`: Visual representation of object counts
- ✅ Printed output in notebook:
  - Total object count by class
  - Frame number with maximum class diversity
- ✅ Annotated frames show bounding boxes and class names (optional)

---

## ⚙️ Setup & How to Run

> You can run this notebook using any Python 3.10+ environment.

### Step 1: (Optional) Create virtual environment
```bash
python -m venv venv
source venv/bin/activate        # Linux/Mac
venv\Scripts\activate           # Windows
````

### Step 2: Install dependencies

```bash
pip install ultralytics opencv-python matplotlib
```

### Step 3: Run the notebook

```bash
jupyter notebook task1.ipynb

---

## 💡 Notes

* The video used is a static metro station exit clip of 10 seconds
* YOLOv5s was used from the `ultralytics` Python package
* The model processed 5th frames only, ensuring efficiency
* Outputs are visible in both notebook and exported PDF

---

## 📫 Contact

**Name:** Gaurav Jha
**Email:** [007gouravjha@gmail.com](mailto:007gouravjha@gmail.com)