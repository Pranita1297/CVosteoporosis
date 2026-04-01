# 🦴 Osteoporosis Classification

## Overview
This project uses deep learning (YOLO classification) to classify X-ray images into:
* Normal
* Osteoporosis
## Problem
Osteoporosis reduces bone density and increases fracture risk. This project aims to classify osteoporosis from X-ray images using AI.
## Dataset
* X-ray images of lower limb / knee
* Dataset split:
  * train
  * valid
  * test
## Method
* Model: YOLO (Ultralytics)
* Task: Image Classification
* Framework: PyTorch
## Project Structure
```
dataset/
├── train/
├── valid/
├── test/
runs/classify/
├── train/
├── train2/
yolo11n-cls.pt
os.ipynb
```
## Installation

```bash
pip install ultralytics torch torchvision
```
## How to Run
### Run in Notebook
Open:
```
os.ipynb
```
and run all cells
### Predict using trained model
```python
from ultralytics import YOLO
model = YOLO("runs/classify/train/weights/best.pt")
results = model.predict("dataset/test/your_image.jpg")
```
## Output Example
```
Prediction: osteoporosis
Confidence: 0.87
```
## Limitations
* Small dataset
* Image quality varies
* Not for medical diagnosis
## Ethics
* Public dataset
* No personal data
* For research/education only

## OUR GROUP
- 67050656 Paphidchaya jaiboon
- 67051278 Apisara Imsap
- 67051292 Pamika Chumpathong
- 67051296 Poonyawe Jitrat
- 67051297 Pranita siritorn

KMITL - Computer Vision Project
