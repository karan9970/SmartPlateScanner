# SmartPlate Scanner using YOLO

## Overview
SmartPlate Scanner is an advanced license plate recognition system that utilizes **YOLO (You Only Look Once)** for real-time number plate detection and OCR for character recognition.

## Features
- Real-time license plate detection using YOLO.
- Optical Character Recognition (OCR) for number extraction.
- High accuracy and fast processing.
- Works on images and video streams.

## Installation
### Prerequisites
Make sure you have the following installed:
- Python 3.7+
- OpenCV
- YOLOv5
- Pytesseract (for OCR)
- NumPy

### Install Dependencies
```bash
pip install -r requirements.txt
```

## Usage
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/smartplate-scanner.git
cd smartplate-scanner
```

### 2. Run the Detector
```bash
python detect.py --source path/to/image_or_video --weights yolov5s.pt
```

### 3. Process the Extracted Plate
```bash
python ocr.py --image path/to/detected_plate
```

## Model Training
To train YOLO on a custom dataset:
```bash
python train.py --img 640 --batch 16 --epochs 50 --data dataset.yaml --weights yolov5s.pt
```

## Output Example
Example of detected license plate:
```
Detected Plate: MH12AB1234
```

## Contributing
Feel free to fork this repository and contribute by submitting a pull request.

## License
This project is licensed under the MIT License.
