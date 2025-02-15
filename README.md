# Retail-object-detection-using-YOLO-v10



## Overview
The **Retail Object Detection System** utilizes **YOLO (You Only Look Once)** to identify and track objects in a retail environment. The system automates checkout by detecting products, generating a unique QR code for each transaction, and providing a web-based interface for customers to view and pay for their purchases online.

## Features
- **Real-time object detection** using YOLO
- **Automatic checkout** with itemized billing
- **QR code generation** for each purchase
- **Web application** for transaction tracking
- **Online payment integration**

## Technologies Used
- **YOLOv8** for object detection
- **OpenCV** for image processing
- **Flask/Django** for web backend
- **React.js/Next.js** for frontend
- **MongoDB/PostgreSQL** for database storage
- **QR Code Generator** (Python library: `qrcode`)
- **Raspberry Pi Model 4B / AMD Kria KR260** for hardware implementation (optional)

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Node.js (if using React for frontend)
- CUDA (for GPU acceleration)
- YOLOv8 (`pip install ultralytics`)
- OpenCV (`pip install opencv-python`)
- Flask/Django (`pip install flask` or `pip install django`)
- Database (MongoDB/PostgreSQL setup)

### Steps to Run the Project
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repo/retail-yolo.git
   cd retail-yolo
   ```
2. **Set up the virtual environment (optional):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the YOLO detection script:**
   ```bash
   python detect.py --source 0  # For webcam input
   ```
5. **Start the web application:**
   ```bash
   python app.py  # If using Flask
   ```
   OR
   ```bash
   python manage.py runserver  # If using Django
   ```
6. **Access the Web UI:**
   Open `http://localhost:5000` or `http://127.0.0.1:8000` in your browser.

## Project Structure
```
retail-yolo/
│── backend/
│   ├── app.py (Flask app) OR manage.py (Django app)
│   ├── models.py
│   ├── routes/
│   └── static/
│── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── index.js
│── object_detection/
│   ├── detect.py
│   ├── yolo_model/
│   └── datasets/
│── qr_code/
│   ├── generate_qr.py
│── requirements.txt
│── README.md
```

## Future Enhancements
- Implement **cloud-based YOLO inference** for scalability
- Add **NFC/RFID integration** for faster checkout
- Deploy as a **mobile application** for enhanced customer experience

## Contributors
- **Your Name** - [karthikeyan yadav](https://github.com/karthikey-yadav)



