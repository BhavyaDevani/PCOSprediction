# PCOS Detection using Ultrasound Images

## Introduction
This repository contains code for a machine learning model to detect Polycystic Ovary Syndrome (PCOS) using ultrasound images. PCOS is a common hormonal disorder among women of reproductive age, and early detection is crucial for effective management.

## Model Overview
The model consists of the following components:

1. Preprocessing: The ultrasound images undergo preprocessing steps to enhance quality and remove noise.
2. Base Models:
   - Xception Model: A pre-trained Xception model is fine-tuned on the dataset to extract features from the ultrasound images.
   - PCOSprediction Model: A custom-trained model specifically designed for PCOS detection, integrated as one of the base models.
3. Ensemble Learning:
   - Stacking Ensemble: A stacking ensemble approach is employed, combining predictions from multiple base models, including PCOSprediction, along with other classifiers.
4. Meta Learner:
   - XGBoost: The meta learner combines the predictions from the base models to generate the final prediction.

## Requirements
- Python 3.x
- TensorFlow
- Keras
- XGBoost
- Other dependencies listed in requirements.txt

## Usage
1. **Data Preparation**: Organize ultrasound images into appropriate directories for training and testing.
2. **Model Training**: Run the training script to train the base models and generate predictions.
3. **Ensemble and Meta Learning**: Implement stacking ensemble and use XGBoost as the meta learner to generate final predictions.
4. **Evaluation**: Evaluate the model performance using relevant metrics.

