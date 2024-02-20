# Jordanian Coin Recognition System

![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![Python](https://img.shields.io/badge/python-3.8-blue.svg)

Automating the detection and classification of Jordanian coins to enhance efficiency and accuracy in financial operations.

## Table of Contents
- [Introduction](#introduction)
- [Challenges](#challenges)
- [Goals](#goals)
- [Methodology](#methodology)

## Introduction
This project addresses the inefficiencies in manual currency handling within businesses, banks, and financial institutions, focusing on the Jordanian currency. By leveraging advanced image recognition technologies, we aim to automate the process of coin detection and classification, thereby reducing time consumption, minimizing human error, and enhancing security.

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/31461bfb-3ebf-4278-8528-d5d8dbb1a8a1)


## Challenges
The manual handling of currency introduces several challenges, including:
- **Time-Consuming Processes:** Extensive manual effort required in counting and detecting currencies.
- **Human Error:** Prone to inaccuracies leading to significant discrepancies.
- **Security Risks:** Increased exposure to theft and fraudulent activities.

## Goals
Our primary objectives include:
1. **Efficient Recognition:** Utilize digital image processing to accurately identify Jordanian coins.
2. **Automated Classification:** Implement classification algorithms for various denominations of Jordanian currency.
3. **Reliable Solution:** Offer a dependable system to replace manual coin inspection, ensuring seamless operations.


## Methodology

Our project follows a comprehensive methodology to develop an effective coin recognition system, covering everything from data collection to model evaluation.

### Data Collection

Our dataset comprises images representing 9 different classes of Jordanian currency, ensuring a wide coverage of denominations for robust model training:

- 5 piasters (5pts)
- 10 piasters (10pts)
- 25 piasters (25pts)
- 50 piasters (50pts)
- 1 Jordanian Dinar (1JD)
- 5 Jordanian Dinars (5JD)
- 10 Jordanian Dinars (10JD)
- 20 Jordanian Dinars (20JD)
- 50 Jordanian Dinars (50JD)

The images were sourced from a variety of settings to capture the diverse conditions under which coins are typically used. To further enhance the dataset, we manually captured additional images using cameras, simulating different environmental conditions to ensure the dataset's comprehensiveness and diversity.

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/a967116a-7f56-4fe9-82fb-8828989452bb)


### Data Augmentation

To address potential class imbalances and enrich the dataset, we employed Roboflow's augmentation capabilities. This approach allowed us to selectively augment images from underrepresented classes, ensuring a balanced dataset that facilitates equitable model training and enhances performance across all currency denominations.

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/69e9d47a-bb3c-4fa3-83a0-ce5b12af085a)
![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/0ed27886-b4a7-4906-aa8d-8f28ce530738)



### Data Splitting

A systematic data splitting strategy was implemented to ensure an optimal balance between training, validation, and testing sets. This approach facilitates a robust assessment of the model's performance and its ability to generalize to new, unseen data.

- **Training Set:** Used to train the model, adjusting the weights and biases to minimize the error between the predicted and actual labels.
- **Validation Set:** Used to tune the model's hyperparameters and prevent overfitting by providing a separate dataset that is not used for training.
- **Testing Set:** Provides a final evaluation of the model's performance, reflecting its ability to generalize to new data.
![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/a38a43e1-ccc9-4bb8-9d08-a2297854fd56)


### Modeling

**Roboflow Model:**
The MS COCO  (Microsoft Common Objects in Context) model by Microsoft is a pre-trained deep learning model utilized for object detection, segmentation, and captioning tasks. Leveraging the MS COCO dataset with annotated images. Renowned for its versatility, it finds applications across various domains, serving as a benchmark in computer vision.

**1- Train from public check point** :
![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/dc5b58ad-61c6-44a9-a552-c17e35867750)

**2- Train from the previous checkpointt** :
![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/0b594c04-8a71-4d11-ae92-42c72393fdc7)



### Evaluation and Testing

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/2b06452a-fdbb-46dc-82ad-602ec8237448)

**Training Cureves**:

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/eb5618c0-3ce8-4470-ac68-711d6e2d26da)

**Losses Curves** :
![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/c97103cb-62d2-4f0c-84ca-ce671709ff73)

**Average Precision by class :**

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/bdc2a957-ef01-48ef-a406-c13a7e8070d2)

### Demo & Counts : 

**Output Samples:**

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/7ea59ab0-0cda-4e13-b131-e2d10fcf6a82)

![image](https://github.com/nooralsmadi/JordanCurrencyDetection/assets/71272030/3214aa36-52cc-40e3-bf07-415814bffb95)





