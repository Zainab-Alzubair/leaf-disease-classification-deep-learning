# Leaf Disease Classification Using Deep Learning and Transfer Learning

## Overview
This project uses deep learning and transfer learning to classify plant leaf images into healthy and diseased plant categories.

The goal is to support early plant disease screening by building an image classification model that can identify visible disease symptoms from leaf images.

## Business Problem
Plant diseases can reduce crop quality and yield. Manual diagnosis may be slow and depends on specialist knowledge, which may not always be available.

This project explores how deep learning can support faster disease screening from leaf images. The model is intended as a decision-support tool, not a replacement for expert diagnosis.

## Dataset
Dataset: New Plant Diseases Dataset  
Source: Kaggle  

The dataset contains labelled RGB images of healthy and diseased plant leaves organized into 38 classes.

The project uses:
- 70,295 training images
- 17,572 validation images
- 38 healthy or disease classes
- Images resized to 128 × 128 pixels before training

## Methods
The project includes:

- Data loading and inspection
- Exploratory data analysis
- Image preprocessing
- CNN model development
- Transfer learning using MobileNetV2
- Model comparison
- Test set evaluation
- Grad-CAM explainability
- Discussion of deployment, business value, and limitations

## Models Compared
- Custom CNN architectures
- MobileNetV2 transfer learning models
- Fine-tuned MobileNetV2 model

## Results
The fine-tuned MobileNetV2 model achieved the best performance:

- Validation accuracy: 96.01%
- Test accuracy: 96.10%

The results show that transfer learning can be effective for plant disease image classification.

## Explainability
Grad-CAM was used to highlight the leaf regions that influenced the model predictions. The model focused mainly on visible disease symptoms such as spots, lesions, and color changes.

## Tools & Technologies
- Python
- NumPy
- pandas
- Matplotlib
- TensorFlow
- Keras
- CNNs
- MobileNetV2
- Transfer Learning
- Grad-CAM
- Google Colab / Jupyter Notebook

## Project Structure
leaf-disease-classification-deep-learning/
├── README.md
├── reports/
│   └── leaf_disease_classification.html
├── notebooks/
│   └── leaf_disease_classification.ipynb
├── requirements.txt
├── .gitignore
└── LICENSE

## How to Run
1. Clone the repository.
2. Install the required Python packages.
3. Download the dataset from Kaggle.
4. Open the notebook in Google Colab or Jupyter Notebook.
5. Run the cells in order.

## Limitations
- The model was trained on controlled images and may perform less accurately on real-world farm photos.
- The model is limited to the 38 classes in the dataset.
- Additional validation on real-world images is needed before deployment.

## Future Improvements
- Test the model on real farm images
- Add more plant disease classes
- Improve deployment readiness
- Build a simple web or mobile app for image prediction
- Add confidence thresholds for uncertain predictions

## Author
Zainab Alzubair  
Data Science, AI, and Digital Marketing student based in Berlin  
LinkedIn: https://www.linkedin.com/in/zainab-alzubair/
