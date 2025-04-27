
# Smart Recycling Assistant

A machine learning project developed during the Samsung Innovation Campus Hackathon.  
This project classifies different types of recyclable waste using a MobileNetV2-based deep learning model.

## Project Overview

- **Goal:** Build an AI model that recognizes recyclable materials (paper, cardboard, plastic, metal, glass) to encourage smarter waste disposal and recycling habits.
- **Value:** Environmental awareness, social education, and financial sustainability.

## Dataset

- Five classes: `paper`, `cardboard`, `plastic`, `metal`, `glass`
- Images are organized into folders by category.

## Model

- **Architecture:**  
  - Pre-trained **MobileNetV2** (frozen weights)  
  - Custom top layers: GlobalAveragePooling2D + Dense output layer
- **Input size:** 224x224 RGB images
- **Loss function:** Categorical Crossentropy
- **Optimizer:** Adam
- **Metrics:** Categorical Accuracy

## Training

- **Batch Size:** 8
- **Epochs:** 14
- **Data Augmentation:** Rotation, zoom, shift, flip
- **Early Stopping:** Configured but optional

## Results

- **Validation Accuracy:** ~88%
- **Test Accuracy:** ~84%
- **Classification Report:**  
  High precision and recall across most classes.

## How to Run

```python
# Mount your Google Drive
from google.colab import drive
drive.mount('/content/drive')

# Follow the notebook steps to load data, preprocess, train, and evaluate the model
```

## Key Libraries

- TensorFlow / Keras
- scikit-learn
- matplotlib
- seaborn
- PIL (Python Imaging Library)

---
