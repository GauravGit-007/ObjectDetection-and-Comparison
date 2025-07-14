# Task 3: YOLOv5 Model Comparison & Deployment

## 🔍 Objective

Compare the performance of two YOLOv5 object detection models — `yolov5n` (nano) and `yolov5s` (small) — on 10 static images, and evaluate:

- 🔹 Inference time
- 🔹 Detection count
- 🔹 Class diversity

---

## 📂 Folder Structure

```

Task3\_ModelComparison/
├── images/                        # 10 test images used
├── outputs/                       # Annotated results from both models
├── task3.ipynb                    # Main Jupyter Notebook
├── task3.html / task3.pdf         # Exported notebook (HTML or PDF)
├── model\_comparison\_results.csv   # Summary table of results
├── Dockerfile                     # Reproducible environment setup
└── README.md                      # Project documentation (this file)

````

---

## 🚀 How to Run

### 📦 Option 1: Run Notebook Locally

1. **Create virtual environment (optional)**:
   ```bash
   python -m venv venv
   venv\Scripts\activate
````

2. **Install dependencies**:

   ```bash
   pip install ultralytics opencv-python matplotlib pandas
   ```

3. **Launch notebook**:

   ```bash
   jupyter notebook task3.ipynb
   ```

---

### 🐳 Option 2: Build and Run with Docker

1. **Build Docker image**:

   ```bash
   docker build -t yolov5-compare .
   ```

2. **Run container (with mounted folder)**:

   ```bash
   docker run --rm -v %cd%:/app yolov5-compare
   ```

   > 💡 On Linux/macOS, replace `%cd%` with `$(pwd)`

3. **This will convert the notebook to HTML inside the container**.

---

## 📌 Notes
* Docker is included for reproducibility but this task was completed in Jupyter Notebook.
* Results are saved in the `outputs/` folder, and summary table in `model_comparison_results.csv`.

---

## 📧 Author

**Gaurav Jha**
Email: \[007gouravjha@gmail.com]
Date: July 2025

