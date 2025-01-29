# chair_dectection_project
 
# Object Detection Using YOLO

## Introduction

This project implements an object detection system using the YOLO (You Only Look Once) model from Ultralytics. The model is capable of detecting multiple objects in images with high accuracy and efficiency. The project utilizes Python, the Ultralytics YOLO library, and PyTorch for deep learning-based detection.

## Features

- **Pre-trained YOLO Model:** Uses a YOLO model trained on COCO dataset.
- **Real-time Object Detection:** Detects objects in images with high speed and efficiency.
- **Easy Setup and Usage:** Simple installation steps with Ultralytics.
- **Image Processing:** Supports multiple image formats for object detection.
- **Customizable Model:** Can be fine-tuned for specific object detection needs.

## Technologies Used

- **Python 3.11** – Programming language for model execution.
- **Ultralytics YOLO** – Pre-trained object detection model.
- **PyTorch** – Deep learning framework for model inference.
- **OpenCV** – Image processing and visualization.

## Installation and Setup

To set up the project locally, follow these steps:

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
   ```

2. **Install the required dependencies:**
   Ensure Python and pip are installed, then run:
   ```sh
   pip install ultralytics
   ```

3. **Check YOLO setup:**
   ```python
   import ultralytics
   ultralytics.checks()
   ```

4. **Download YOLO model and test with a sample image:**
   ```python
   from ultralytics import YOLO
   model = YOLO("yolo11n.pt")
   results = model("zidane.jpg")
   ```

## Sample Output

When the script runs, it detects objects in an image and provides details such as detection confidence and processing time:

```
Ultralytics 8.3.69 🚀 Python-3.11.11 torch-2.5.1+cu121 CPU (Intel Xeon 2.20GHz)
Setup complete ✅ (2 CPUs, 12.7 GB RAM, 31.3/107.7 GB disk)

detecting objects...
image 1/1 /content/zidane.jpg: 384x640 2 persons, 1 tie, 161.6ms
Speed: 16.5ms preprocess, 161.6ms inference, 36.5ms postprocess per image.
Results saved to runs/detect/predict
```

## Usage Guide

1. **Prepare your images:** Place images in the appropriate directory.
2. **Run the detection script:** Execute the notebook to process and detect objects in the images.
3. **View results:** The detected images with bounding boxes are saved in the `runs/detect/predict` directory.

## Potential Applications

- **Autonomous Vehicles:** Object detection for navigation and obstacle avoidance.
- **Security Surveillance:** Monitoring real-time camera feeds for unauthorized objects.
- **Retail Analytics:** Detecting customer movement patterns in stores.
- **Medical Imaging:** Identifying objects in X-ray and MRI scans.

