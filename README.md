# Mobile-Price-Prediction-project-
# 📱 Mobile Price Classification Using Machine Learning

## 📌 Project Overview

This project focuses on predicting mobile phone price categories using Machine Learning classification algorithms. The prediction is based on various mobile specifications, including RAM, battery capacity, internal memory, screen dimensions, camera features, connectivity, and processing capabilities.

The project follows a complete machine learning workflow, starting from data exploration and preprocessing to model training, hyperparameter tuning, and performance evaluation.

## 🎯 Project Objectives

- Analyze mobile phone specifications using Exploratory Data Analysis (EDA).
- Identify important features influencing mobile price categories.
- Perform data cleaning and preprocessing.
- Explore relationships between mobile specifications and price ranges.
- Build multiclass classification models.
- Optimize model performance using hyperparameter tuning.
- Compare different machine learning algorithms.

## 📂 Dataset Information

- **Dataset:** Mobile Price Classification
- **Total Records:** 2,000
- **Total Features:** 20 input features + 1 target variable.
- **Target Variable:** `price_range`
- **Problem Type:** Multiclass Classification

### Target Categories

| Price Range | Category |
|---|---|
| 0 | Low Cost |
| 1 | Medium Cost |
| 2 | High Cost |
| 3 | Very High Cost |

### Important Features

- `battery_power` – Battery capacity.
- `ram` – Random Access Memory.
- `int_memory` – Internal memory.
- `mobile_wt` – Mobile weight.
- `px_height` – Pixel resolution height.
- `px_width` – Pixel resolution width.
- `fc` – Front camera megapixels.
- `pc` – Primary camera megapixels.
- `four_g` – 4G availability.
- `three_g` – 3G availability.
- `dual_sim` – Dual SIM availability.
- `wifi` – Wi-Fi availability.

## 🛠️ Technologies & Libraries

**Programming Language**
- Python

**Data Analysis**
- Pandas
- NumPy

**Data Visualization**
- Matplotlib
- Seaborn

**Machine Learning**
- Scikit-learn

**Development Environment**
- Jupyter Notebook / Google Colab

## 🔍 Project Workflow

### 1. Data Loading
- Imported the dataset using Pandas.
- Inspected dataset dimensions and column names.
- Examined data types and initial records.

### 2. Data Cleaning and Preprocessing
- Checked missing values.
- Identified duplicate records.
- Examined unique values.
- Checked invalid pixel and screen dimensions.
- Detected potential outliers using the IQR method.
- Removed selected records with invalid zero values.

### 3. Exploratory Data Analysis (EDA)
- Analyzed descriptive statistics.
- Examined feature distributions and percentiles.
- Compared average RAM, battery power, screen resolution, and memory across price categories.
- Analyzed camera specifications.
- Investigated 3G, 4G, and touchscreen availability.
- Performed correlation analysis.

### 4. Data Visualization
- Created count plots for price categories.
- Compared 3G and 4G availability across price categories.
- Used correlation analysis to understand relationships between features.

### 5. Machine Learning Models

Implemented the following classification algorithms:

**Logistic Regression**
- Developed a multiclass classification model.
- Split the dataset into training and testing sets.
- Evaluated training and testing accuracy.

**Decision Tree Classifier**
- Built a Decision Tree classification model.
- Applied GridSearchCV for hyperparameter tuning.
- Evaluated the optimized model.

**Random Forest Classifier**
- Developed an ensemble classification model.
- Tuned model parameters using GridSearchCV.
- Evaluated classification performance.

### 6. Model Evaluation

The models are evaluated using:

- Accuracy Score
- Training Accuracy
- Testing Accuracy
- Classification Report
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Cross-Validation Accuracy

## ⚙️ Hyperparameter Tuning

GridSearchCV with 5-fold cross-validation is used for Decision Tree and Random Forest models.

The tuning process explores parameters such as:

- Maximum tree depth
- Number of estimators
- Minimum samples split
- Minimum samples leaf
- Splitting criterion
- Maximum features

## 📊 Expected Outcome

The project aims to develop a multiclass classification system that predicts whether a mobile phone belongs to a low, medium, high, or very high price category based on its technical specifications.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Place the CSV dataset in the project directory.
4. Open the Jupyter Notebook.
5. Execute the notebook cells sequentially.
6. Review the EDA visualizations and model evaluation results.

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## 📁 Project Structure

```text
Mobile-Price-Classification/
│
├── mobile_price.csv
├── mobileML.ipynb
└── README.md
```

## 👨‍💻 Author

**Mohammad Asad**

B.Sc. (Prog.) Applied Physical Sciences with Computer Science

Interests: Data Analytics | Machine Learning | Data Science | Data Visualization

## 📌 Key Learning Outcomes

- Practical experience in data preprocessing and EDA.
- Understanding multiclass classification.
- Implementation of multiple machine learning algorithms.
- Hyperparameter optimization using GridSearchCV.
- Model evaluation and performance comparison.
- Building an end-to-end machine learning workflow.
