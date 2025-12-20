---

# AI Self-Checkout System using YOLO

## Overview

This project implements a **simple AI-based self-checkout system** using **YOLO object detection**.
The system detects products placed in a checkout area using a camera and automatically generates a bill without using barcodes or RFID.

The project is intended as a **baseline implementation** for academic projects, demos, and research in computer vision–based retail automation.

---

## Objectives

* Detect products using a YOLO model
* Identify and count products automatically
* Generate a simple bill based on detected items
* Perform detection in real time using a single camera

---

## System Architecture

Camera Input
↓
YOLO Object Detection
↓
Product Identification
↓
Item Counting
↓
Bill Generation

---

## Technologies Used

* Python
* YOLO (YOLOv8 / YOLOv10)
* OpenCV
* PyTorch
* Ultralytics Framework

---

## Project Structure

self-checkout/
│
├── data/
│   ├── train/
│   └── val/
│
├── weights/
│   └── yolo_model.pt
│
├── main.py
├── requirements.txt
└── README.md

---

## Dataset

* Custom product images (fruits, packaged goods, etc.)
* Annotated in YOLO format
* Images captured under real checkout conditions
* Split into training and validation sets

---

## Installation

1. Clone the repository
   git clone [https://github.com/your-username/self-checkout-yolo.git](https://github.com/your-username/self-checkout-yolo.git)
   cd self-checkout-yolo

2. Install dependencies
   pip install -r requirements.txt

---

## How It Works

1. The camera captures live video of the checkout area
2. YOLO detects products in each frame
3. Detected products are mapped to predefined prices
4. Items entering the checkout area are added to the cart
5. The total bill is displayed in real time

---

## Output

* Bounding boxes around detected products
* Product name and quantity
* Total bill amount displayed on the screen

---

## Features

* Real-time object detection
* No barcode or RFID required
* Camera-only solution
* Simple and lightweight implementation
* Easy to extend for research or deployment

---

## Limitations

* Detection accuracy depends on lighting conditions
* Occlusions can affect counting accuracy
* Similar-looking products may be misclassified
* Payment gateway is not integrated

---

## Future Improvements

* Add object tracking for better counting
* Handle occlusions using temporal logic
* Integrate QR code or UPI payment system
* Deploy on edge devices like Jetson Nano
* Improve accuracy with larger datasets

---

## Applications

* Retail self-checkout counters
* Smart stores
* Automated billing systems
* Academic and research projects

---

## Conclusion

This project demonstrates a **simple and effective AI self-checkout system using YOLO**.
It serves as a strong **baseline** for further enhancements such as tracking, payment integration, and edge deployment.

---

If you want, I can also:

* Convert this into **paper-style documentation**
* Make it **YOLOv10-specific**
* Add a **Results and Metrics section**
* Rewrite it for **final-year project submission**

Just tell me.
