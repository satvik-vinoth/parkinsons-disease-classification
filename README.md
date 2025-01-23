# Parkinson's Disease Classification using CNN
This repository contains a Python-based implementation of a convolutional neural network (CNN) to classify MRI images into two categories: Non-PD Patients and PD Patients. The model predicts whether an MRI scan indicates Parkinson's Disease (PD).

## Features
 - Preprocesses MRI images by resizing, normalizing, and assigning binary labels.
 - A custom CNN model with convolutional, batch normalization, dropout, and fully connected layers.
 - Binary classification using Binary Cross-Entropy Loss and Adam optimizer.
 - Training and validation loss/accuracy tracking for performance monitoring.

## Dataset

The dataset used in this project is the NTUA Parkinson Dataset, which includes MRI scans of 150 subjects:
 - 75 Parkinson's Disease (PD) patients.
 - 75 healthy controls.

The dataset is organized into two categories: Non PD Patients and PD Patients.

Download the dataset from the following link: [NTUA Parkinson Dataset](https://www.kaggle.com/datasets/shayalvaghasiya/ntua-prakinson)

```plaintext
ntua-parkinson-dataset-master/
├── Non PD Patients/
│   ├── Patient1/
│   │   └── 1.MRI/
│   │       ├── image1.png
│   │       └── image2.png
│   └── ...
├── PD Patients/
│   ├── Patient1/
│   │   └── 1.MRI/
│   │       ├── image1.png
│   │       └── image2.png
│   └── ...
```

## Model Architecture
The CNN model consists of:
 - Convolutional Layers: Three convolutional layers for feature extraction.
 - Batch Normalization: Normalizes feature maps to stabilize learning.
 - MaxPooling: Reduces spatial dimensions.
 - Dropout: Regularization to prevent overfitting.
 - Fully Connected Layers: For binary classification.
 - Sigmoid Activation: Outputs probability for binary labels.

## **How to Use**

1. **Clone this repository**:
   ```bash
   git clone https://github.com/satvik-vinoth/parkinsons-disease-classification.git
   ```
2. Navigate to the project directory:
   ```bash
   cd parkinsons-disease-classification
   ```
3. Run the Jupyter Notebook:
  ```bash
jupyter notebook Parkinson_disease_classification.ipynb
```

## Outputs

1) Training Logs:
 - Epoch-wise training and validation loss/accuracy.
2) Plots:
 - Loss vs. Epoch.
 - Accuracy vs. Epoch.
 - Confusion Matrix.
 - ROC Curve.
 - Precision-Recall Curve.

## Results

 - Training Accuracy: 98.07 %
 - Validation Accuracy: 97.35 %

## Contact
For questions, feel free to reach out via GitHub.





