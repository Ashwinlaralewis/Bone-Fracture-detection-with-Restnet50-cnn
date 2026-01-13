Bone Fracture Detection Using CNN (ResNet-50)
Overview

Bone fracture detection from X-ray images is a critical task in medical diagnosis. Manual examination can be time-consuming and prone to error.
This project implements an automated bone fracture detection system using Convolutional Neural Networks (CNN) with a ResNet-50 architecture to classify X-ray images as Fractured or Normal.

The system also provides a Graphical User Interface (GUI) that allows users to upload an X-ray image and receive real-time predictions.

Key Features

CNN-based bone fracture classification

Transfer learning using pretrained ResNet-50

Binary classification: Fracture vs Normal

Image preprocessing and normalization

Simple and user-friendly GUI application

Suitable for academic and research purposes

Dataset

X-ray images of human bones

Two classes:

Fracture

Normal

Images resized to 224 × 224

Dataset split into training and testing sets

Data augmentation applied to improve model generalization

Publicly available datasets (e.g., Kaggle or MURA-style datasets) can be used.

Model Architecture

Base model: ResNet-50

Pretrained on ImageNet

Custom fully connected layers added

Sigmoid activation for binary classification

Optimizer: Adam

Loss function: Binary Cross-Entropy

Technologies Used

Python 3.x

TensorFlow / Keras

NumPy

OpenCV

Pillow

Tkinter (GUI)

Matplotlib

Scikit-learn

Project Workflow

Load and preprocess X-ray images

Resize and normalize input data

Apply data augmentation

Train ResNet-50 model

Evaluate model performance

Save trained model

Perform prediction using GUI

Installation
Clone the Repository
git clone https://github.com/your-username/bone-fracture-detection.git
cd bone-fracture-detection

Install Dependencies
pip install -r requirements.txt


⚠️ Recommended Python version: Python 3.8 – 3.10
(Newer versions may cause compatibility issues with some libraries)

Running the Application (GUI)

After installing the dependencies, run the GUI application using:

python mainGUI.py

Using the GUI

Launch the application

Click Upload Image to select an X-ray image

The image is automatically preprocessed

Click Predict / Detect Fracture

The result is displayed as:

Fracture

Normal

Prediction confidence may also be shown (if enabled)

Model Performance

Typical performance metrics:

Accuracy: ~90% (varies with dataset)

Precision: High

Recall: High

F1-Score: Balanced

Performance depends on dataset quality, size, and training configuration.

Folder Structure
bone-fracture-detection/
│
├── dataset/
│   ├── train/
│   ├── test/
│
├── models/
│   └── resnet50_model.h5
│
├── train.py
├── test.py
├── predict.py
├── mainGUI.py
├── requirements.txt
└── README.md
