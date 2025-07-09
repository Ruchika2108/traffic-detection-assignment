# 🚦 Traffic Vehicle Detection System

A computer vision-based project using **YOLOv8** to automatically detect, classify, and count vehicles (cars, trucks, motorcycles) in traffic images. Built as part of an internship assessment, this project focuses on detection accuracy, clean outputs, and a user-friendly interface.

---

## 📌 Table of Contents

* Overview
* Features
* Project Structure
* Requirements
* Installation
* Usage
* Sample Results
* System Architecture
* About the Developer

---

## 🔍 Overview

This project uses the **YOLOv8** model (via Ultralytics) for object detection. The system can detect vehicles in images, classify them by type (car, truck, motorcycle), and output both annotated media and a CSV report. A Gradio-based interface allows easy real-time interaction.

---

## ✨ Features

* ✅ Detects Cars, Trucks, and Motorcycles
* ✅ Displays Confidence Scores with Bounding Boxes
* ✅ Color-Coded Boxes per Vehicle Type
* ✅ Saves Annotated Images
* ✅ CSV Summary for Vehicle Counts
* ✅ Gradio Web App with Image and Video Support

---

## 📁 Project Structure

```
traffic-detection-assignment/
├── README.md
├── requirements.txt
├── Traffic_Vehicle_Detectionnn.ipynb
├── data/
│   └── test_images/
│       ├── test1.jpg
│       ├── test2.jpg
│       └── test3.jpg
├── output/
│   └── processed_images/
│       ├── sample1.jpg
│       ├── sample2.jpg
│       └── sample3.jpg
│   └── vehicle_counts_summary.csv
└── docs/
    ├── technical_report.pdf
    └── presentation_slides.pdf
```

---

## ⚙️ Requirements

Install all dependencies via:

```bash
pip install -r requirements.txt
```

**Libraries Used:**

* ultralytics
* opencv-python
* numpy
* pandas
* matplotlib
* tqdm
* gradio
* Pillow

---

## 💻 Installation

Clone this repo locally:

```bash
git clone https://github.com/your-username/traffic-detection-assignment.git
cd traffic-detection-assignment
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Open and run the notebook:

```bash
Traffic_Vehicle_Detectionnn.ipynb
```

This will:

* Load images from `data/test_images/`
* Annotate vehicles using YOLOv8
* Save outputs to `output/processed_images/`
* Create a summary file: `vehicle_counts_summary.csv`

To launch the Gradio interface, run the final cell.

---

## 📊 Sample Results

**🖼️ Test Images:**

* `test1.jpg`, `test2.jpg`, `test3.jpg` in `data/test_images/`

**✅ Output Samples:**

* `sample1.jpg`, `sample2.jpg`, `sample3.jpg` in `output/processed_images/`

**📄 CSV Preview:**

```
Image Name    Cars   Trucks   Motorcycles   Total
test1.jpg       2       1         0           3
test2.jpg       1       0         2           3
```

---

## 🧠 System Architecture

```mermaid
flowchart TD
    A[Input Images] --> B[YOLOv8 Detection]
    B --> C[Bounding Boxes + Confidence Scores]
    C --> D[Save Annotated Image]
    B --> E[Vehicle Counting]
    E --> F[CSV Summary Generation]
```

---

## 🙋‍♀️ About the Developer

**Ruchika Sarode**
B.Tech Artificial Intelligence Student, Nagpur
📧 [sruchika162@gmail.com](mailto:sruchika162@gmail.com)
