# Money Detection using YOLOv8

Python-based application that utilizes the YOLOv8 object detection model to identify and highlight currency (banknotes and coins) in images. It reads images, detects money objects using a pre-trained YOLOv8 model, and outputs annotated images with bounding boxes and confidence scores. The program also provides statistics on the number of detected money objects.

*Note: used YOLOv8 model is not pre-trained to specifically detect money (banknotes or coins). To more accurately detect money, model could be pre-trained on a dataset (for example, on https://universe.roboflow.com/tatmantech/worldwide_currency,  https://www.kaggle.com/datasets/wanderdust/coin-images/data or another dataset).*

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

1. Update the `image_path` in `detect_money()` in ```money_detector.ipynb``` with your image file path.
2. Run cells in same file ```money_detector.ipynb``` to see detected results and statistics.
