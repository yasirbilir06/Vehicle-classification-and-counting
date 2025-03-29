# Vehicle Classification and Counting System using YOLOv8

This project is a deep learning-based image processing system developed to classify vehicles and count them accurately from traffic videos. It uses a custom-trained YOLOv8 model along with the BYTETracker algorithm to ensure reliable object tracking and avoid duplicate counting.

## 🎯 Project Objective

To improve traffic efficiency by detecting, classifying, and counting different types of vehicles from video data. The system is designed for use in traffic analysis, parking management, and intelligent transportation systems.

## 🧠 Key Features

- Custom dataset with 830 annotated images labeled via Roboflow
- YOLOv8 object detection model trained on 11 vehicle classes
- ByteTrack tracking algorithm to assign unique IDs and prevent recounting
- Frame-based vehicle tracking from pre-recorded 10-minute traffic footage
- Google Colab-based training environment with GPU support
- Line-crossing logic to count vehicles only once

## 🛠️ Technologies Used

- Python 3
- [YOLOv8](https://github.com/ultralytics/ultralytics)
- [BYTETracker](https://github.com/ifzhang/ByteTrack)
- [Roboflow](https://roboflow.com/)
- OpenCV
- NumPy & Pandas
- Google Colab (T4 GPU)
- Supervision library (for annotations)
- Matplotlib (for visualizations)

## 🗂️ Classes in Dataset

1. Cargo Minivan  
2. Cargo Van  
3. Motorcycle  
4. Passenger Van  
5. Pedestrian  
6. Pickup Truck  
7. Taxi  
8. Tractor Trailer  
9. Bicycle  
10. Bus  
11. Cars  

## 📊 Model Performance

- **mAP**: 77.0%  
- **Precision**: 79.1%  
- **Recall**: 66.3%

## 📈 Example Use Cases

- Traffic density analysis in urban areas
- Smart parking management systems
- Real-time vehicle monitoring and reporting
- Infrastructure planning for smart cities
- Support for autonomous vehicle algorithms

## 📹 Sample Workflow

1. Record a traffic video (e.g. 10 minutes)
2. Extract frames and label using Roboflow
3. Train YOLOv8 model on custom dataset via Colab
4. Apply line-crossing logic to count vehicles
5. Use ByteTrack to assign unique IDs per object
6. Visualize and export results

## 📁 Folder Structure (Suggested)
├── dataset/
│   └── annotated_images/
├── yolo_training/
│   └── yolov8_training.ipynb
├── vehicle_counting/
│   └── object_tracking_bytrack.py
├── results/
│   └── output_videos/
├── README.md


## ✍️ Author

**Muhammed Yasir Bilir**  
Selçuk University – Department of Computer Engineering  
Bitirme Projesi (Graduation Thesis), 2025

---

> _This repository showcases a complete AI pipeline from data preparation to model training and deployment, highlighting how deep learning can solve real-world problems in traffic analysis._



