# OpenVINO-Webcam-Object-Detection

# OpenVINO Object Detection with Webcam

This repository contains a simple Python script for real-time object detection using the OpenVINO toolkit. The script captures video frames from the webcam, processes them through a pre-trained model, and displays the results.

## Prerequisites

Make sure you have the following dependencies installed:

- OpenVINO 2022.3
- Python (>=3.6)
- opencv-python
- numpy

You can install the required Python packages using the following command:

```bash
pip install opencv-python numpy
```

## Setup

1. Clone the repository:

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

2. Download the OpenVINO model files (`.xml` and `.bin`) and label file. Update the file paths in the script accordingly.

3. Run the script:

```bash
python openvino_detector.py
```

## Script Overview

The `openvino_detector.py` script performs the following steps:

1. Imports necessary modules and classes, including OpenVINO, OpenCV, and numpy.
2. Reads the model and compiles it using the OpenVINO Core.
3. Initializes a webcam using OpenCV and sets up a loop to continuously capture frames.
4. Resizes and preprocesses each frame for input to the model.
5. Performs inference using the compiled model.
6. Displays the processed frame with bounding boxes and class labels.
7. Listens to keyboard input to exit the application (press 'Esc').

## Performance Metrics

The script includes a `PerformanceMetrics` class to measure the execution time of each frame processing iteration. This can be useful for assessing the real-time performance of the object detection pipeline.

## Note

Make sure to replace the placeholder paths and filenames with the actual paths to your model files and label file.

Feel free to customize the script according to your requirements and use case.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
