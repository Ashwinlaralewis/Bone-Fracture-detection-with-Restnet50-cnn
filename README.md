Bone Fracture Detection Using CNN (ResNet-50)
📌 Overview

Bone fracture diagnosis using radiographic (X-ray) images is a critical task in medical imaging. This project presents an automated bone fracture detection system using deep learning, specifically a Convolutional Neural Network (CNN) based on ResNet-50.

The model classifies X-ray images into fractured and non-fractured categories, assisting radiologists by improving diagnostic accuracy and reducing manual effort.

🧠 Model Architecture – ResNet-50

Pretrained ResNet-50 model

Transfer learning using ImageNet weights

Custom fully connected layers added for binary classification

Residual connections help prevent vanishing gradients

📂 Dataset

This project uses publicly available musculoskeletal X-ray images.

Key features:

Grayscale X-ray images

Binary classes: Fracture and Normal

Images resized to 224 × 224

Data augmentation applied to improve generalization

Example sources:

MURA Dataset

Kaggle bone fracture datasets

⚙️ Project Workflow

Data Loading & Preprocessing

Image Augmentation

Model Building (ResNet-50)

Training & Validation

Model Evaluation

Prediction on New X-ray Images

🧪 Technologies Used

Python 3.x

TensorFlow / Keras

NumPy

OpenCV

Matplotlib

Scikit-learn

🚀 Installation & Setup
# Clone the repository
git clone https://github.com/your-username/bone-fracture-detection.git

# Navigate to the project directory
cd bone-fracture-detection

# Install dependencies
pip install -r requirements.txt
