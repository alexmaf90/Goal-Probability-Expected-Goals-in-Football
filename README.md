## Description

This project predicts the probability of a football goal using a Logistic Regression model trained on StatsBomb historical data. With over 20,000 shots and various explanatory variables, the analysis explores the dynamics influencing successful shots.

## Table of Contents

- [Data](#data)
- [Features](#features)
- [Models](#models)
- [Results](#results)

### Data
The dataset, sourced from StatsBomb, includes 20,000+ shots, providing insights into player positioning, goalkeeper distance, and goal angle.

### Features
Explanatory variables in the Logistic Regression model include player positioning, goalkeeper distance, and goal angle. 
Key variables are the number of players in the shooter's field of vision, distance to the goalkeeper, and distance to the nearest player.

### Models

In the context of this project, Expected Goals (xG) is fundamentally a classification problem. The classification arises from predicting whether a given shot will result in a goal or not. 
By framing it as a binary classification problem (goal or no goal), the model can effectively learn and discern the key factors influencing successful goal attempts.

We explore various binary classification models:

1. **Logistic Regression:** Used as a baseline, it provides a foundation for improvement in different metrics.
2. **Random Forest:** 
3. **XGBoost:** 
4. **Decision Tree:** 
5. **Support Vector Machine (SVM):**

### Model Evaluation

In the evaluation of both models, the logistic regression model stood out despite XGBoost exhibiting a higher accuracy. This decision was rooted in the comprehensive assessment of various performance metrics, ultimately highlighting the logistic regression model's superior discriminative capability.

- **ROC AUC:** The logistic regression model outperformed with a higher score of 0.79, signifying a better ability to distinguish between positive and negative instances.

- **Recall:** The logistic regression model demonstrated commendable performance with a substantially higher recall score of 0.69, indicating its proficiency in capturing true positive goal events.

- **F1 Score:** The logistic regression model was favored in the F1 score, striking a balance between precision and recall and indicating a more harmonized approach in correctly identifying goal outcomes.

In addition to these metrics, the logistic regression model offers a notable advantage in terms of explainability. This characteristic is of paramount importance, providing insights into the underlying factors influencing the model's predictions, thereby enhancing interpretability and trustworthiness.

Hence, despite a seemingly higher accuracy for the XGBoost model, the logistic regression model was the preferred choice due to its superior performance in critical metrics, better alignment with the project's specific objectives, and its enhanced explainability all pivotal factors in achieving accurate and meaningful predictions.

### Results
The model exhibited good performance, particularly in recall for actual goal instances.
Key variables influencing goal probabilities include the number of players in the shooter's field of vision, distance to the goalkeeper, and distance to the nearest player.
Areas with the highest goal probability are central regions of the penalty area and near the goal.
Comparison with the StatsBomb model showed superior performance, especially in terms of recall for actual goal instances.

