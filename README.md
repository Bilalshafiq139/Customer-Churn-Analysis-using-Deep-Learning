# Customer-Churn-Analysis-using-Deep-Learning
This repository contains a Python script that implements Customer Churn Prediction using a Deep Learning Neural Network.



## Overview
This repository contains a Python script that implements **Customer Churn Prediction** using a **Deep Learning Neural Network**. The model predicts whether a customer will churn (leave the service) based on various demographic and account-related factors.

---

## **Problem Statement**
Customer churn is a significant issue for businesses, as retaining existing customers is more cost-effective than acquiring new ones. This project builds a **binary classification model** using **Deep Learning (Neural Networks)** to predict customer churn based on historical data.

### **Dataset Description**
The dataset used in this project is from [**Kaggle: Churn Modelling Dataset**](https://www.kaggle.com/datasets/mathchi/churn-for-bank-customers) and includes features such as:
- **Customer Demographics** (Age, Gender, Geography)
- **Account Information** (Credit Score, Balance, Tenure)
- **Activity Metrics** (Number of Products, Active Membership, Estimated Salary)
- **Exited (Target Variable)**:
  - `1`: Customer churned.
  - `0`: Customer retained.

---

## **How the Script Works**
1. **Data Preprocessing**:
   - Loads the dataset and removes unnecessary columns (`RowNumber`, `CustomerId`, `Surname`).
   - Converts categorical features (`Geography`, `Gender`) into numerical values using **One-Hot Encoding**.
2. **Feature Scaling**:
   - Uses **StandardScaler** to normalize numerical features.
3. **Train-Test Split**:
   - Splits the dataset into **80% training** and **20% testing**.
4. **Neural Network Model Architecture**:
   - **Input Layer**: 11 features.
   - **Hidden Layer**: 3 neurons, **Sigmoid activation**.
   - **Output Layer**: 1 neuron, **Sigmoid activation** (for binary classification).
5. **Model Compilation & Training**:
   - Uses **Binary Cross-Entropy Loss**.
   - Optimizes using **Adam Optimizer**.
   - Trains for **100 epochs**.
6. **Model Evaluation**:
   - Computes **Accuracy Score**.
   - Plots **Loss vs. Validation Loss** curve.
7. **Prediction**:
   - Uses a probability threshold of `0.5` to classify customers as churned or retained.

---

## **Dependencies**
Ensure you have the following Python libraries installed:
```sh
pip install numpy pandas tensorflow scikit-learn matplotlib
```

---

## **How to Run the Script**
1. Clone the repository:
   ```sh
   git clone <repository_url>
   ```
2. Navigate to the project folder:
   ```sh
   cd <project_folder>
   ```
3. Run the Python script:
   ```sh
   python churn_analysis_deep_learning_campusx.py
   ```
4. Follow the output to view accuracy and predictions.

---

## **Contributing**
Contributions are welcome! Feel free to fork this repository and submit a pull request with improvements or additional features.

