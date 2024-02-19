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

### Data Augmentation

To address potential class imbalances and enrich the dataset, we employed Roboflow's augmentation capabilities. This approach allowed us to selectively augment images from underrepresented classes, ensuring a balanced dataset that facilitates equitable model training and enhances performance across all currency denominations.

### Data Splitting

A systematic data splitting strategy was implemented to ensure an optimal balance between training, validation, and testing sets. This approach facilitates a robust assessment of the model's performance and its ability to generalize to new, unseen data.

- **Training Set:** Used to train the model, adjusting the weights and biases to minimize the error between the predicted and actual labels.
- **Validation Set:** Used to tune the model's hyperparameters and prevent overfitting by providing a separate dataset that is not used for training.
- **Testing Set:** Provides a final evaluation of the model's performance, reflecting its ability to generalize to new data.

### Modeling



### Evaluation and Testing

