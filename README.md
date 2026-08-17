# Multi-task-Learning_mentalhealth-Socialmedia
Machine learning project analyzing the relationship between social media usage, lifestyle factors, and happiness, with a Random Forest-based Happiness Index predictor.
# Mental Health & Social Media Balance

## 📌 Project Overview

This project analyzes the relationship between **social media usage, lifestyle factors, and happiness** using Python and machine learning.

The dataset contains **500 records and 10 attributes**, including age, gender, daily screen time, sleep quality, stress level, days without social media, exercise frequency, social media platform, and happiness index.
The project performs exploratory data analysis and develops regression models to predict the **Happiness Index (1–10)**.

## 🎯 Objectives

* Analyze social media usage and lifestyle patterns.
* Explore factors associated with the Happiness Index.
* Perform exploratory data analysis and visualization.
* Build machine learning regression models.
* Compare model performance using R², RMSE, and MAE.
* Develop an interactive Happiness Predictor.

## 📊 Dataset Features

The dataset includes:

* `User_ID`
* `Age`
* `Gender`
* `Daily_Screen_Time(hrs)`
* `Sleep_Quality(1-10)`
* `Stress_Level(1-10)`
* `Days_Without_Social_Media`
* `Exercise_Frequency(week)`
* `Social_Media_Platform`
* `Happiness_Index(1-10)`

The notebook also checks data types and missing values; the displayed missing-value analysis shows zero missing values across the listed attributes.

## 🔍 Machine Learning Approach

The following features are used as model inputs:

* Daily Screen Time
* Sleep Quality
* Stress Level
* Days Without Social Media
* Exercise Frequency

The target variable is:

* **Happiness Index**

The data is divided into training and testing sets using an 80:20 split with `random_state=42`.

## 🤖 Models Used

### 1. Linear Regression

A baseline regression model used to establish a performance benchmark.

### 2. Random Forest Regressor

An ensemble learning model using 200 decision trees.

### 3. Gradient Boosting Regressor

A boosting-based regression model using 200 estimators and a learning rate of 0.05.

## 📈 Model Performance

| Model             |  R² Score |      RMSE |       MAE |
| ----------------- | --------: | --------: | --------: |
| Linear Regression |     0.611 |     0.962 |     0.814 |
| Random Forest     | **0.636** | **0.930** | **0.748** |
| Gradient Boosting |     0.627 |     0.941 |     0.762 |

Based on the notebook results, **Random Forest performed best** across the three reported evaluation metrics.

## 💡 Interactive Happiness Predictor

The notebook includes a user-interactive prediction function that accepts lifestyle inputs such as:

* Daily screen time
* Sleep quality
* Stress level
* Days without social media
* Exercise frequency
* Most-used social media platform

It then predicts the Happiness Index and provides a simple happiness-level classification and lifestyle suggestions.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Statsmodels
* Jupyter Notebook / Google Colab

## 📁 Project Structure

```text
Mental-Health-Social-Media-Balance/
│
├── Mental_Health_&_Social_Media_Balance.ipynb
├── README.md
└── dataset/
    └── Mental_Health_and_Social_Media_Balance_Dataset.csv
```

## 🚀 How to Run

1. Clone or download this repository.
2. Open the `.ipynb` file using Jupyter Notebook, JupyterLab, or Google Colab.
3. Install the required Python libraries if necessary.
4. Update the dataset path in the notebook.
5. Run the notebook cells sequentially.

## 📌 Key Result

The analysis compares three regression approaches, with **Random Forest achieving the strongest reported performance** with an R² score of approximately **0.636** and an MAE of approximately **0.748**.

## ⚠️ Disclaimer

This project is intended for **educational and analytical purposes**. The predicted Happiness Index should not be interpreted as a clinical or psychological assessment.

## 👩‍💻 Author

**Bhakthi MD**

M.Tech – Data Science / Machine Learning
