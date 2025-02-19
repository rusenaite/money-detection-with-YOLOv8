# Money Detector using YOLOv8

Python-based application that utilizes the YOLOv8 object detection model to identify and highlight currency (banknotes and coins) in images. It reads images, detects money objects using a pre-trained YOLOv8 model, and outputs annotated images with bounding boxes and confidence scores. The program also provides statistics on the number of detected money objects.

## Features

- Detects and labels monetary objects in an image.
- Outputs a new image with detected objects highlighted.
- Provides statistics on detection count and confidence.

## Requirements

Required libraries and packages to run the project:
- OpenCV
- Ultralytics YOLO
- Matplotlib

## Usage

1. Update the `image_path` in `detect_money()` with your image file path.
2. Run the script to see detected results and statistics.
