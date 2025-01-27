# Handwritten Digit Recognition Using CNN

This repository demonstrates a **Convolutional Neural Network (CNN)** implementation for recognizing handwritten digits using the **MNIST dataset**. The project involves data preprocessing, CNN construction, training, evaluation, and saving the trained model for reuse or deployment.

---

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Model Deployment](#model-deployment)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

Handwritten digit recognition is a classic problem in computer vision, with applications in postal services, banking, and OCR systems. This project provides a simple yet effective way to classify handwritten digits (0-9) using CNNs, leveraging the MNIST dataset.

---

## Dataset

The **MNIST dataset** contains:
- **60,000** training images.
- **10,000** test images.

Each image is grayscale with a resolution of **28x28 pixels**, representing a single digit.

---

## Features

- **CNN Architecture**: Includes convolutional, max-pooling, and dense layers for feature extraction and classification.
- **Data Normalization**: Preprocesses input data for better convergence.
- **Training & Evaluation**: Trains the model on MNIST data and evaluates its performance.
- **Model Saving**: Saves the trained model as a `.h5` file.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/musharafhussainabid/CNN_Handwritten_Digit_Recognition_System.git
   cd CNN_Handwritten_Digit_Recognition_System
   ```

2. Install the required dependencies:
   ```bash
   pip install tensorflow numpy matplotlib opencv-python
   ```

3. (Optional) If running on Google Colab, mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

---

## Usage

### 1. Train the Model
Run the script to train the CNN:
```bash
python hand_digit_recognition_using_cnn.ipynb
```

### 2. Evaluate the Model
After training, the script evaluates the model's accuracy and loss on the test set.

### 3. Save the Model
The trained model is saved as `cnn-hand-digit-recognition-system.h5` in the specified directory.

---

## Results

- **Loss**: Final test loss 0.05.
- **Accuracy**: Final test accuracy 98%.
- Achieved high accuracy on MNIST with a simple CNN.

---

## Model Deployment

The trained model can be loaded and used for predictions:
```python
from tensorflow.keras.models import load_model

model = load_model('cnn-hand-digit-recognition-system.h5')
```

---

## Contributing

Contributions are welcome! If you have ideas to improve this project or extend its functionality, please fork the repository and submit a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
