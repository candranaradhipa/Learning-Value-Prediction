# Learning Value Evaluation Prediction Using RNN Methods

## Overview
This project develops a machine learning-based student grade prediction system using historical academic data. The proposed system is designed to predict students' academic performance more accurately, support efficient learning evaluation, and provide valuable insights that assist educators in making informed academic decisions.

## Requirements & Tools
The following tools and requirements were used throughout the system development and implementation process:
- Python 3 Environments
- Jupyter Notebook
- pandas
- numpy
- scikit-learn
- torch
- seaborn
- tensorflow

## Dataset 
A CSV-formatted dataset obtained from Kaggle, named data.csv, was used. The dataset contains several attributes employed as research variables, including `1st` to `5th`, which represent students' academic grades for each semester, `College Code`, which indicates the institution code, `Gender`, which specifies the student's gender, and `Code Subject`, which represents the course code.

## Usage
1. **Data Preparation and Preprocessing**
   The dataset is prepared and selected, typically in **CSV** format, before being integrated into the program. Subsequently, preprocessing is performed to clean, organize, and transform the data into a suitable format for the subsequent stages of the study.

2. **Training and Testing Data**
   The dataset is divided into two subsets: **training data** and **testing data**. The training data are used to train the model over a predetermined number of **epochs**, while the testing data are employed to evaluate the model's ability to make predictions on previously unseen data.

3. **Visualization**
   The prediction and evaluation results are presented through visualizations. These visualizations facilitate the interpretation of the model's performance and provide insights into its predictive capability and overall accuracy.

## Results 📊
Correlation analysis using a heatmap and scatter plot revealed a strong relationship between the Grade Point Averages (GPAs) from semesters 1 to 4 and the GPA in semester 5. This finding indicates that students' academic performance in previous semesters can serve as a reliable basis for predicting their academic performance in subsequent semesters.
<img width="915" height="796" alt="image" src="https://github.com/user-attachments/assets/31d59930-bc9a-4671-b1cf-81d3ee61db14" />

### Regression Analysis
After confirming the relationship among the variables, three prediction models—Linear Regression, RNN, and LSTM—were evaluated using the MSE, MAE, and RMSE metrics to measure prediction errors. Lower error values indicate better model performance and higher prediction accuracy.

### Performance Evaluation
After confirming the relationship among the variables, three prediction models—Linear Regression, RNN, and LSTM—were evaluated using the MSE, MAE, and RMSE metrics to measure prediction errors. Lower error values indicate better model performance and higher prediction accuracy.

| Model | MSE ↓ | MAE ↓ | RMSE ↓ |
|:------------------|------:|------:|------:|
| **Linear Regression** | **0.1858** | **0.3411** | **0.4311** |
| LSTM | 0.2143 | 0.3701 | 0.4630 |
| RNN | 0.2201 | 0.3786 | 0.4692 |

### Visual Evaluation
The prediction visualization shows that the Linear Regression model produces a curve that most closely matches the actual data compared to the RNN and LSTM models. This observation is consistent with the evaluation results based on MSE, MAE, and RMSE, confirming that Linear Regression achieved the best predictive performance on the dataset.

<img width="886" height="711" alt="image" src="https://github.com/user-attachments/assets/46a51c46-21d6-4b04-beac-60767309da76" />
<img width="915" height="592" alt="image" src="https://github.com/user-attachments/assets/235eb127-6940-4c5c-8689-547f2a69fa94" />
<img width="915" height="592" alt="image" src="https://github.com/user-attachments/assets/4e3ad9eb-af3d-423d-8c5d-37bf0c79ac64" />
