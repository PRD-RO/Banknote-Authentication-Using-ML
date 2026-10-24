# **CS 435 - Machine Learning Project**
## **Project Title: Banknote Authentication Using Machine Learning**

---

## **Overview**
Counterfeit currency poses a major threat to financial systems and the global economy. This project aims to build and evaluate robust binary classification models to detect forged (fake) banknotes versus genuine ones using statistical features extracted from digitized banknote images. We compare the performance of a linear model (**Logistic Regression**) against a non-linear model (**Decision Tree Classifier**)[cite: 6].

---

## **Dataset Information**
The dataset used in this project (`BankNote_Authentication.csv`) consists of **1,372 instances** with 5 columns[cite: 6]:
* **variance**: Variance of Wavelet Transformed image (Continuous)[cite: 6]
* **skewness**: Skewness of Wavelet Transformed image (Continuous)[cite: 6]
* **curtosis**: Curtosis of Wavelet Transformed image (Continuous)[cite: 6]
* **entropy**: Entropy of image (Continuous)[cite: 6]
* **class**: Target variable where `0` represents a **Genuine** banknote and `1` represents a **Counterfeit** banknote[cite: 6].

---

## **Project Workflow**
1. **Data Loading & Inspection**: Importing the dataset, inspecting data types, checking shapes, and generating statistical summaries[cite: 6].
2. **Exploratory Data Analysis (EDA)**: Checking for missing values and visualizing class distributions[cite: 6].
3. **Data Preprocessing & Scaling**: 
   * Splitting features ($X$) and target labels ($y$)[cite: 6].
   * Applying **StandardScaler** to normalize features to a zero mean and unit variance[cite: 6].
4. **Train/Test Split**: Partitioning the dataset into training and testing sets (80% train, 20% test) with stratified sampling[cite: 6].
5. **Model Training & Evaluation**:
   * **Logistic Regression**: A linear classification approach[cite: 6].
   * **Decision Tree Classifier**: A non-linear tree-based approach[cite: 6].
6. **Performance Metrics**: Evaluating models using **Accuracy**, **Precision**, **Recall**, **F1-Score**, and **Confusion Matrices**[cite: 6].

---

## **Prerequisites & Libraries**
Make sure you have the following Python libraries installed before running the notebook[cite: 6]:

```bash
pip install pandas seaborn matplotlib scikit-learn
```
## **Model Performance Summary**
Logistic Regression: Achieved an overall Accuracy of ~97.09%[cite: 6].

Decision Tree Classifier: Outperformed the linear model with an Accuracy of ~99.27% due to its ability to capture complex non-linear decision boundaries[cite: 6].

## **Repository Structure**
├── BankNote_Authentication.csv   # The dataset file
├── banknote_project.ipynb        # Main Google Colab / Jupyter Notebook
└── README.md                     # Project Documentation

Developed as part of the CS 435 Machine Learning coursework.
