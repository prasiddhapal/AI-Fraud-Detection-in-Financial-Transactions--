# 💳 AI-Powered Fraud Detection in Financial Transactions

### 🔐 *"Catch the Fraud Before It Strikes!"*

> 🚀 Developed with ❤️ by **PRASIDDHA PAL**

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Dataset Information](#dataset-information)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Results & Insights](#results--insights)
- [Future Enhancements](#future-enhancements)
- [Acknowledgements](#acknowledgements)

---

## 📘 Project Overview

This machine learning project detects fraudulent financial transactions with high accuracy by analyzing transaction patterns in real-world anonymized credit card data. The model leverages advanced classification techniques to identify suspicious activities and minimize false positives while maximizing fraud detection.

**Problem Statement:** With millions of transactions happening daily, manual fraud detection is inefficient. This project automates the process using machine learning to protect customers and financial institutions.

---

## ✨ Key Features

- 🎯 **High Accuracy Detection** - ~99.8% overall accuracy
- ⚖️ **Handles Imbalanced Data** - Only 0.17% of transactions are fraudulent
- 🔍 **Feature Importance Analysis** - Identifies top fraud indicators
- 📊 **Comprehensive Evaluation** - Includes confusion matrix, classification reports
- 🧪 **Production-Ready** - Well-documented, reproducible pipeline
- 📈 **Explainable Results** - Clear visualization of model decisions

---

## 🧠 Tech Stack

| Component | Technologies |
|-----------|---------------|
| **Language** | 🐍 Python 3.8+ |
| **Data Processing** | 📊 Pandas, NumPy |
| **Machine Learning** | 🤖 Scikit-learn (Random Forest Classifier) |
| **Visualization** | 📉 Matplotlib, Seaborn |
| **Notebook** | 💻 Jupyter Notebook / Google Colab |

---

## 🗂️ Project Structure

```
AI-Fraud-Detection-in-Financial-Transactions--/
│
├── 📓 ai_fraud_detection.ipynb      # Main Jupyter notebook with full pipeline
├── 📊 creditcard.csv                 # Dataset (download separately)
├── 📄 README.md                      # Project documentation (this file)
└── 📝 .gitignore                     # Git ignore file
```

---

## 📊 Dataset Information

| Property | Details |
|----------|---------|
| **Name** | Credit Card Fraud Detection Dataset |
| **Source** | [Kaggle - ULB ML Group](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) |
| **Size** | 284,807 transactions |
| **Features** | 30 features (V1-V28 + Time + Amount) |
| **Class Distribution** | 99.83% legitimate, 0.17% fraudulent (highly imbalanced) |
| **License** | Open Data - Please credit ULB ML Group if used |

### ⚠️ Important: Dataset Not Included

The dataset is not included in this repository due to size and licensing constraints.

**👉 [Download from Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)** and place `creditcard.csv` in the root directory.

---

## 🛠️ Installation & Setup

### Prerequisites

- Python 3.8 or higher
- pip or conda package manager
- Jupyter Notebook or Google Colab

### Step 1: Clone the Repository

```bash
git clone https://github.com/prasiddhapal/AI-Fraud-Detection-in-Financial-Transactions--.git
cd AI-Fraud-Detection-in-Financial-Transactions--
```

### Step 2: Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Step 3: Download Dataset

1. Visit [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
2. Download `creditcard.csv`
3. Place it in the project root directory

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook ai_fraud_detection.ipynb
```

---

## 🚀 Usage

### Running Locally

1. Open `ai_fraud_detection.ipynb` in Jupyter Notebook
2. Run cells sequentially (Shift + Enter)
3. The notebook will:
   - Load and explore the dataset
   - Preprocess and scale features
   - Train the Random Forest classifier
   - Evaluate performance with detailed metrics
   - Display feature importance and visualizations

### Running on Google Colab

1. Upload `ai_fraud_detection.ipynb` to Google Colab
2. Upload `creditcard.csv` when prompted
3. Run the notebook cells

### Expected Output

- ✅ Trained Random Forest model
- 📊 Confusion matrix visualization
- 📈 ROC curve and classification reports
- 🔹 Feature importance plot
- 📋 Detailed performance metrics

---

## 📊 Model Performance

### Classification Metrics

| Metric | Value |
|--------|-------|
| **Accuracy** | ~99.8% |
| **Precision (Fraud Class)** | ~92% |
| **Recall (Fraud Class)** | ~64% |
| **F1-Score (Fraud Class)** | ~76% |
| **ROC-AUC Score** | ~0.97 |

### What These Metrics Mean

- 🎯 **Accuracy:** How often the model is correct overall
- 🔍 **Precision:** When the model predicts fraud, how often is it right? (92%)
- 🔁 **Recall:** Of all actual frauds, how many did the model catch? (64%)
- 📊 **Confusion Matrix:** Breakdown of True Positives, False Positives, True Negatives, False Negatives

---

## 🌟 Results & Insights

### Top Features for Detecting Fraud

The model identified these as the most important fraud indicators:

1. 🔹 **V14** - Most discriminative feature
2. 🔹 **V10** - Second most important
3. 🔹 **V12** - Consistent fraud signal
4. 🔹 **V17** - Notable fraud indicator
5. 🔹 **V4** - Supplementary feature

*Note: Features V1-V28 are PCA-transformed components of original transaction data (anonymized for privacy)*

### Key Observations

- 💡 The dataset is highly imbalanced, requiring careful evaluation metrics
- 💡 Transaction amount and timing patterns are valuable fraud signals
- 💡 Random Forest effectively captures non-linear relationships
- 💡 Model achieves excellent precision (fewer false alarms for customers)

---

## 🚀 Future Enhancements

- [ ] ⚙️ Implement SMOTE/ADASYN for improved imbalance handling
- [ ] 🌲 Experiment with XGBoost, LightGBM, and ensemble methods
- [ ] 🔄 Add cross-validation for robust performance estimation
- [ ] 🌐 Deploy as REST API (Flask/FastAPI)
- [ ] 🖥️ Build web dashboard with Streamlit
- [ ] 📡 Implement real-time fraud detection pipeline
- [ ] 🧪 Add explainability features (SHAP, LIME)
- [ ] 📚 Create production-grade model pipeline (MLflow, DVC)

---

## 🔗 Useful Resources

- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Random Forest Classifier Guide](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [Imbalanced Data Handling](https://imbalanced-learn.org/)
- [Credit Card Fraud Detection - Research Paper](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

## 📝 License

This project is open source. Please credit the **ULB Machine Learning Group** for the dataset and **PRASIDDHA PAL** for the implementation.

---

## 🙏 Acknowledgements

- 📊 **Dataset:** ULB Machine Learning Group - [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- 📚 **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
- 🎓 **Inspiration:** Machine Learning and Financial Security communities

---

## 📞 Contact & Contributions

**Author:** PRASIDDHA PAL  
**GitHub:** [@prasiddhapal](https://github.com/prasiddhapal)

### Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

### 👨‍💻 Built with passion and ❤️

*Last Updated: 2026*
