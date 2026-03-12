# AI-Based Network Intrusion Detection System

An **AI-powered Network Intrusion Detection System (NIDS)** that detects malicious network traffic using **Machine Learning and Neural Networks**.
The project analyzes network flow data and classifies traffic as **normal or attack**.

The system is implemented in **Python using Scikit-learn and deep learning techniques** and is trained on the **UNSW-NB15 cybersecurity dataset**.

---

# Project Overview

Cybersecurity threats are increasing rapidly, and manual monitoring of network traffic is inefficient.

This project builds an **automated intrusion detection system** that can:

* Analyze network traffic features
* Detect malicious activity
* Classify attacks using machine learning
* Assist in real-time cybersecurity monitoring

---

# Dataset

The project uses the **UNSW-NB15 dataset**, a widely used dataset for intrusion detection research.

The dataset contains:

* Network flow features
* Protocol information
* Packet statistics
* Attack labels

Files used:

* `UNSW_NB15_training-set.parquet`
* `UNSW_NB15_testing-set.parquet`

The target variable:

```
label
```

* **0 → Normal Traffic**
* **1 → Attack**

---

# Project Workflow

The system follows a complete **machine learning pipeline**.

## 1. Data Loading

Network traffic datasets are loaded using **Pandas**.

```
pd.read_parquet()
```

Training and testing datasets are separated.

---

## 2. Data Cleaning

Steps performed:

* Remove unnecessary columns
* Drop `attack_cat`
* Check missing values
* Remove duplicates

---

## 3. Exploratory Data Analysis (EDA)

EDA is performed to understand the dataset.

Analysis includes:

* Dataset structure
* Null value detection
* Duplicate record detection
* Class distribution visualization

Visualization tools used:

* Matplotlib
* Seaborn

Example visualization:

* Attack vs Normal traffic distribution

---

## 4. Data Preprocessing

Preprocessing steps include:

* Encoding categorical variables
* Feature scaling using **StandardScaler**
* Splitting features and target variables

---

## 5. Train-Test Split

The dataset is divided into:

```
Training Data
Testing Data
```

Using:

```
train_test_split()
```

---

## 6. Model Training

Machine learning models are trained to classify traffic.

Models may include:

* Logistic Regression
* Random Forest
* Neural Networks

The goal is to learn patterns that distinguish **normal traffic from malicious traffic**.

---

## 7. Model Evaluation

The model performance is evaluated using:

* Accuracy
* Confusion Matrix
* Classification Report

These metrics help measure how well the model detects intrusions.

---

# Technologies Used

Programming Language:

* Python

Libraries:

* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

Machine Learning Techniques:

* Supervised Learning
* Feature Scaling
* Classification Algorithms

Dataset Format:

* Parquet

---

# Project Structure

```
AI-Network-Intrusion-Detection
│
├── AI_Project.ipynb
├── UNSW_NB15_training-set.parquet
├── UNSW_NB15_testing-set.parquet
└── README.md
```

---

# Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/AI-Network-Intrusion-Detection.git
```

Navigate to the project folder:

```bash
cd AI-Network-Intrusion-Detection
```

Install dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn pyarrow
```

---

# Running the Project

Open the notebook:

```bash
jupyter notebook AI_Project.ipynb
```

Run all cells to:

1. Load dataset
2. Perform EDA
3. Train machine learning models
4. Evaluate intrusion detection performance

---

# Applications

This project can be used for:

* Network security monitoring
* Intrusion detection systems
* Cybersecurity research
* AI-based threat detection

---

# Future Improvements

Possible enhancements:

* Deep Learning models (CNN / LSTM)
* Real-time packet monitoring
* Deployment as a **web-based intrusion detection dashboard**
* Integration with **SIEM systems**

---

# Author

Adarsh Sharma
