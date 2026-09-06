# AI-Intrusion-Detection
content = """# AI Network Intrusion Detection System

## Overview
This project is a Machine Learning model designed to classify network traffic as either `Normal` or `Malicious` (Attack). It serves as a foundational implementation of an AI-powered Intrusion Detection System (IDS).

## Dataset
The model is trained on the **NSL-KDD** dataset, which is a standard benchmark for network security evaluation. It contains network connection records, detailing features like protocol types, login attempts, and byte transfers.

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas
* **Machine Learning:** Scikit-Learn (Random Forest Classifier)
* **Environment:** Google Colab / Jupyter Notebook

## Project Workflow (Methodology)
This project followed a standard data science pipeline:
1. **Data Loading:** Retrieved the raw text data directly into a Pandas DataFrame.
2. **Data Cleaning & Structuring:** Mapped the 43 column names to the raw data for readability.
3. **Feature Engineering (Encoding):** 
   * Converted text-based categories (like `protocol_type` TCP/UDP) into numerical representations using One-Hot Encoding so the algorithm could process them.
   * Converted the target column (`attack_type`) into a binary classification: `0` for normal traffic and `1` for any type of cyber attack (e.g., Neptune, Smurf, Satan).
4. **Train/Test Split:** Divided the data (80% training, 20% testing) to ensure the model was evaluated on unseen network traffic.
5. **Model Training:** Utilized a **Random Forest Classifier**, which builds multiple decision trees and uses majority voting to prevent overfitting.
6. **Evaluation:** Scored the model using Accuracy, Precision, and Recall metrics.

## How to Run
1. Open the notebook file in Google Colab or your local Jupyter environment.
2. Run the cells sequentially to load the dataset, preprocess the data, and train the model.
3. The final cell will output the model's accuracy and the classification report.
"""
