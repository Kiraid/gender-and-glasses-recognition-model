# Custom Neural Network for Multi-Label Image Classification

A **custom multi-output neural network** built to classify two attributes from facial images:  
1. **Gender** (Male / Female)  
2. **Presence of Glasses** (Yes / No)  

The dataset was **scraped from iStock** and manually labeled.  
The model achieved **76% accuracy** on gender classification and **86% accuracy** on glasses detection.

---

## Project Overview

This project demonstrates:
- **Data scraping** and **manual labeling** for custom dataset creation.
- **Multi-output neural network architecture** in Keras/TensorFlow.
- End-to-end pipeline: data preprocessing, exploratory analysis, model training, evaluation, and visualization.
- Handling **two classification tasks** simultaneously.

---

##  Tech Stack

**Languages & Libraries**
- Python
- Pandas (data loading & preprocessing)
- Seaborn (exploratory data visualization)
- Keras & TensorFlow (deep learning model)

---

##  Dataset

- **Source**: Scraped from [iStock](https://www.istockphoto.com/).
- **Size**: Custom (manually curated and labeled).
- **Labels**:
  - `gender`: `male` / `female`
  - `glasses`: `yes` / `no`
- **Format**: JPEG images organized in directories, with a CSV file for labels.

---

##  Exploratory Data Analysis (EDA)

- **Class balance checks** for gender and glasses categories.
- **Visual inspection** of sample images.
- **Distribution plots** created using Seaborn to identify potential bias in the dataset.

---

## Model Architecture

- **Type**: Multi-output Convolutional Neural Network (CNN)
- **Base Layers**: Convolution + MaxPooling
- **Flatten & Dense Layers** for feature extraction.
- **Two output layers**:
  - Output 1: Gender classification (`softmax`)
  - Output 2: Glasses detection (`sigmoid`)

---

## Results

| Task                | Accuracy |
|---------------------|----------|
| Gender Classification | 76%      |
| Glasses Detection     | 86%      |

---


