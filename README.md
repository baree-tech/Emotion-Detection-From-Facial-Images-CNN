### Emotion Detection from Facial Images using CNN

## Overview
This project builds a CNN model for emotion recognition from grayscale facial images. The model achieves up to *72.23% accuracy* and is built entirely in TensorFlow/Keras using the FER-2013 dataset.

**Note:** All outputs- sample images,training accuracy/loss graphs, confusion matrix, classification report, and sample predictions are already included in the notebook itself. No need to run the entire code again unless you wish to retrain the model again.

## Dataset
- Dataset: FER-2013 (Facial Expression Recognition)
- Grayscale images: 48x48 px
- Classes: ['Angry', 'Disgust', 'Fear', 'Happy', 'Sad', 'Surprise', 'Neutral']

## Model Architecture
- 3 Convolutional blocks with MaxPooling
- BatchNormalization and Dropout
- Flatten and Dense layers
- Softmax output with 7 units

## Training Strategy
- Loss: categorical_crossentropy
- Optimizer: Adam
- EarlyStopping (patience=5)
- ReduceLROnPlateau (monitor='val_loss', patience=2, min_lr=1e-5)
- Epochs: 50 (stopped early at 16)

## Evaluation
- Training Accuracy: 72.23%
- Validation Accuracy: 58.47%
- Visualizations: 
  - Accuracy vs Epoch
  - Loss vs Epoch
  - Confusion Matrix
  - Sample Images with Labels
  - sample images with predictions

## Future Work
- Implement *Transfer Learning* using pre-trained CNN architectures (e.g., VGG16, MobileNetV2)
- Data Augmentation
- Improve class balance

## Run the Code
```bash
Run on Google Colab (Python 3.11, TensorFlow 2.x)

##Created By Bareera Mushthak
Aspiring AI Engineer

Connect With Me
	•	LinkedIn: www.linkedin.com/in/bareera-mushthak
	•	GitHub: https://github.com/baree-tech

--Thank you for visiting my repository--
