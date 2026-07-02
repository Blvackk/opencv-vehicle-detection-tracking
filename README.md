# opencv-vehicle-detection-tracking
Vehicle detection and multi-object tracking using OpenCV, Background Subtraction (MOG2), and Euclidean Distance Tracking.

# 🚗 Vehicle Detection and Tracking using OpenCV

A Computer Vision project that detects and tracks moving vehicles in a highway video using **OpenCV**, **Background Subtraction (MOG2)**, **Contour Detection**, and a custom **Euclidean Distance Tracker**. Each detected vehicle is assigned a unique ID, enabling consistent tracking across video frames.

---

## 📖 Overview

Vehicle detection and tracking are fundamental tasks in intelligent transportation systems, traffic monitoring, and video surveillance. This project demonstrates how classical computer vision techniques can be used to identify and track multiple moving vehicles without relying on deep learning models.

The application processes a highway traffic video, extracts moving objects using background subtraction, detects vehicle contours, and tracks each vehicle by assigning a unique identifier based on the Euclidean distance between object centroids.

---

## ✨ Features

- 🎥 Detects moving vehicles from a highway traffic video
- 🚗 Tracks multiple vehicles simultaneously
- 🆔 Assigns unique IDs to detected vehicles
- 📍 Tracks vehicle movement across consecutive frames
- 🎯 Uses Region of Interest (ROI) to improve detection efficiency
- 🔥 Background subtraction using MOG2
- 📦 Contour-based object detection
- 🟩 Draws bounding boxes around detected vehicles
- ⚡ Lightweight implementation using OpenCV

---

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Computer Vision:** OpenCV
- **Numerical Computing:** NumPy

---

## 📂 Project Structure

```text
opencv-vehicle-detection-tracking/
│
├── highway.mp4
├── main.py
├── tracker.py
├── Video_capture.py
├── White_mask.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Blvackk/opencv-vehicle-detection-tracking.git
```

```bash
cd opencv-vehicle-detection-tracking
```

### 2. (Optional) Create a Virtual Environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux/macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

### Play the Input Video

```bash
python Video_capture.py
```

### Generate the Foreground Mask

```bash
python White_mask.py
```

### Detect and Track Vehicles

```bash
python main.py
```

---

## ⚙️ How It Works

The vehicle detection and tracking pipeline consists of the following steps:

1. Read frames from the highway traffic video.
2. Extract the Region of Interest (ROI).
3. Apply Background Subtraction (MOG2) to separate moving objects from the background.
4. Convert the foreground into a binary mask using thresholding.
5. Detect contours representing moving vehicles.
6. Filter contours based on area to eliminate noise.
7. Compute bounding boxes around detected vehicles.
8. Track vehicles using a Euclidean Distance Tracker.
9. Assign and maintain unique IDs for each tracked vehicle.
10. Display the processed video with tracking information.

---

## 📊 Workflow

```text
Highway Video
      │
      ▼
Video Capture
      │
      ▼
Region of Interest (ROI)
      │
      ▼
Background Subtraction (MOG2)
      │
      ▼
Binary Thresholding
      │
      ▼
Contour Detection
      │
      ▼
Bounding Box Generation
      │
      ▼
Euclidean Distance Tracking
      │
      ▼
Vehicle ID Assignment
      │
      ▼
Tracked Vehicle Display
```

---

## 📌 Future Improvements

- Vehicle counting
- Vehicle speed estimation
- Lane detection
- Traffic density analysis
- Real-time webcam support
- YOLOv8-based vehicle detection
- DeepSORT or ByteTrack integration
- Vehicle classification (Car, Bus, Truck, Bike)
- Automatic incident detection

---

## 🎯 Learning Outcomes

This project demonstrates practical knowledge of:

- Computer Vision fundamentals
- OpenCV video processing
- Background subtraction
- Contour detection
- Region of Interest (ROI)
- Multi-object tracking
- Euclidean distance-based tracking
- Bounding box generation
- Real-time video analysis

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

## 👨‍💻 Author

**Pratik Lagishetty**

- GitHub: https://github.com/Blvackk

---

## ⭐ Support

If you found this project useful, please consider giving it a **⭐ Star**. It helps others discover the project and motivates future improvements.

---

## 📄 License

This project is licensed under the MIT License.
