# Money Detection using YOLOv8

This project consists of two different money detection implementations using YOLOv8:

1. **Pre-trained YOLOv8 model** – Detects money (banknotes and coins) but lacks accuracy in distinguishing between them.
2. **Custom-trained YOLOv8 model** – Trained on a specialized dataset from Roboflow to improve recognition of banknotes and coins.

## Features
- Detects and labels money objects in images.
- Outputs an annotated image with detected objects.
- Provides statistics on the number of detected banknotes and coins.
- Custom-trained model offers better recognition for different currency types.

## Methods and Libraries Used
- **YOLOv8**: Object detection framework by Ultralytics.
- **Roboflow Dataset**: Custom-trained model uses a dataset downloaded via:
https://universe.roboflow.com/tatmantech/worldwide_currency   
- **OpenCV**: Image processing and visualization.
- **Matplotlib**: Visualization of detection results.

## System Description
- **Pre-trained YOLOv8 model** detects money but lacks precision, often misclassifying coins and banknotes.
- **Custom-trained YOLOv8 model** improves accuracy using a dataset from Roboflow.
- The program reads an image, applies the YOLOv8 model, and generates an output image with bounding boxes.
- Example output from the trained model:
  ```
  0: 480x640 1 1, 2 100s, 3 banknotes, 40.6ms
  ```

## Issues and Solutions
- **Problem:** Pre-trained YOLOv8 model does not recognize money accurately.
  - **Solution:** A dataset from Roboflow was used to train a custom model.
- **Problem:** Low confidence in coin detection.
  - **Possible Solution:** More training data and fine-tuning were used to improve classification.

## How to Run the System
### **Running the Pre-Trained YOLOv8 Model**
1. Install required dependencies:
   ```bash
   pip install ultralytics opencv-python matplotlib
   ```
2. Open `money_detection_with_yolov8.ipynb`.
3. Update `image_path` with the path to your image file.
4. Run the notebook to detect money and visualize results.

### **Running the Custom-Trained YOLOv8 Model**
1. Install required dependencies:
   ```bash
   pip install ultralytics opencv-python roboflow matplotlib
   ```
4. Open `banknote-detection-with-trained-model.ipynb` and update `image_path` with your test image.
5. Run the notebook to perform detection using the trained model.
