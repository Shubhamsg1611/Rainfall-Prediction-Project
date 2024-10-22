# Rainfall-Prediction-Project
![rainfall](https://github.com/Shubhamsg1611/Rainfall-Prediction-Project/blob/main/Banner%20Image.jpg)

### Overview:
In this rainfall prediction project, you applied machine learning techniques, particularly logistic regression, to predict whether it will rain tomorrow based on historical weather data. The dataset includes various weather-related features like temperature, humidity, wind speed, and atmospheric pressure, as well as the target variable RainTomorrow (1 for rain, 0 for no rain).

#### Key Steps in the Project:
1. Data Preprocessing:- Handled missing values and outliers in the dataset.
- Encoded categorical variables and performed feature scaling to prepare the data for modeling.

2.Train-Test Split:
- The dataset was split into training and test sets (80%-20%) to ensure proper model evaluation.

3.Addressing Class Imbalance:
- Since the dataset was imbalanced (more no-rain days than rain days), the SMOTE (Synthetic Minority Over-sampling Technique) method was used to balance the classes.

4. Model Training:
- A logistic regression model was trained on the balanced dataset to predict the likelihood of rain.

5. Model Evaluation:
- The model's performance was evaluated using accuracy, precision, recall, F1 score, and confusion matrix.

#### Model Performance:
- Accuracy: 77.62%: The model correctly predicted whether it will rain tomorrow in 77.62% of cases.
- Precision for Rain (1.0): 47.71%: Of all the days the model predicted rain, 47.71% were correct. This relatively low precision suggests a high number of false positives (days predicted as rain when it didn’t rain).
- Recall for Rain (1.0): 75.12%: The model correctly identified 75.12% of the actual rain days, indicating good recall, which is crucial for rain prediction.
- F1 Score: 58.35%: This score balances precision and recall, showing that the model’s ability to predict rain can still be improved.
- Confusion Matrix: The model performed well on predicting no rain days (class 0), but struggled with predicting rain days (class 1), leading to false positives.

#### Conclusion:
The logistic regression model demonstrated reasonable overall accuracy, but it struggled with predicting rain, as evidenced by the low precision for rainy days. The recall was decent, meaning the model caught most of the actual rain days, but at the cost of a high number of false positives.
