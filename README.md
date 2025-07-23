# 🌾 Crop Disease Detection

A machine learning solution for **crop disease identification** using **leaf images**, built with deep learning and deployed via a simple API/web app.

## 📌 Project Overview

- **Goal**: Detect various crop diseases from leaf images (e.g., mildew, rust) to help farmers with quick diagnostics.
- **Approach**: Image classification using CNN-based models (e.g., transfer learning with MobileNet/VGG).
- **Features**:
  - Handles multiple plant and disease types
  - Simple interface for image input and prediction output

## 📁 Repository Contents

- `models/` – Pre-trained model weights
- `data/` – Sample leaf images organized by disease class
- `train.py` – Script to train or fine-tune the classification model
- `predict.py` – Prediction script for individual leaf images
- `app/` – (Optional) Web or API deployment using Flask/Django
- `requirements.txt` – Python dependencies

## 🧠 Getting Started

### Setup

1. Clone the repo and navigate in:
   
   git clone https://github.com/KancharlaSindhupriya/CROP-DISEASE.git
   
   cd CROP-DISEASE

2. Install dependencies:

   pip install -r requirements.txt
   
### Training

Modify hyperparameters in `train.py`, then run:

python train.py \
  --epochs 20 \
  --batch_size 32 \
  --img_size 224 \
  --data_dir ./data


### Prediction

Use the trained model to predict:

python predict.py --model models/crop_disease.h5 --image test/leaf.jpg

Output:

Predicted disease: Tomato___Late_blight (Confidence: 92.4%)

## 🛠️ Tech Stack

* **Python**, TensorFlow/Keras or PyTorch
* **CNN Architectures**: MobileNet, VGG, etc.
* **Data Augmentation**: Flip, rotation, scaling
* **Deployment**: Flask REST API or web interface


## 📈 Performance & Results

* Trained on [PlantVillage-style dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset) (≈50k leaf images, 14 crops, 26 disease types)

* Achieves \~95%–99% accuracy depending on the model and augmentation

## 👩‍💻 About You

**Sindhupriya Kancharla**
Data Scientist & ML Intern
📧 [sindhupriyakancharla04@gmail.com](mailto:sindhupriyakancharla04@gmail.com)
🔗 [GitHub](https://github.com/KancharlaSindhupriya) | [LinkedIn](https://linkedin.com/in/sindhupriyakancharla)


