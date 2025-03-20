# Decision Trees Analysis for Alcohol Consumption Prediction 🍷🔍

## Overview
This project presents a comprehensive analysis using decision trees in R to predict alcohol consumption based on biometric and demographic data. Developed as part of the "TD VI: Artificial Intelligence" course (2nd Semester, 2024) by Luca Mazzarello and Camila Migdal, the work is documented in an R Markdown file that integrates code, visualizations, results, and detailed explanations.

## Project Structure
The analysis is organized into the following sections:

1. **Introduction to the Problem**  
   - Overview of the dataset, its origin (sourced from Kaggle), and the key variables.
   - Justification for choosing decision trees given the mix of numerical and categorical predictors and the non-linear relationships inherent in the data.

2. **Data Preparation**  
   - Data loading and preprocessing, including transformation of numerical codes into categorical labels.
   - Exploratory Data Analysis (EDA) with descriptive statistics and visualizations (e.g., box plots for Gamma-GTP, SGOT/AST, and Triglycerides).

3. **Basic Decision Tree Construction**  
   - Splitting the dataset into training (70%), validation (15%), and test (15%) sets.
   - Building an initial decision tree using R’s **rpart** package.
   - Interpretation of the tree structure and the decision rules generated.

4. **Evaluation of the Basic Decision Tree**  
   - Generating predictions and calculating key performance metrics:
     - Confusion Matrix, Accuracy, Precision, Recall, F1-Score, and AUC-ROC.
   - Analyzing the results to assess the model's strengths and limitations.

5. **Model Optimization**  
   - Experimenting with different hyperparameters (max depth, min split, and min bucket) to improve the model's performance.
   - Visualizing the relationship between hyperparameters and AUC-ROC.
   - Comparing the performance of the basic and optimized models.

6. **Interpretation of Results**  
   - Visual comparison of the basic and optimized trees.
   - Analysis of variable importance, highlighting predictors such as gamma-GTP, hemoglobin, and age.

7. **Impact of Missing Values**  
   - Generating three new datasets with 20%, 50%, and 75% missing values (NAs).
   - Re-optimizing the model for each case and comparing performance metrics to understand how missing data impacts the model.

8. **Conclusions and Discussion**  
   - Summarizing key findings and discussing the effectiveness of decision trees for this binary classification problem.
   - Highlighting areas for future improvement, such as exploring ensemble methods like Random Forests or Boosting to mitigate issues with missing data and enhance model robustness.

## Tools and Libraries Used
- **R and R Markdown** for reproducible research.
- **rpart** for constructing decision trees.
- **ggplot2** for creating informative visualizations.
- **caret** and **pROC** for model evaluation.
- Additional libraries: **dplyr**, **reshape2**, and **scales**.

## How to Run the Analysis
1. **Open the R Markdown file** (e.g., `TP1_TDVI.Rmd`).
2. **Install the necessary packages** in R if you haven’t already (e.g., rpart, ggplot2, caret, pROC).
3. **Knit the R Markdown file** to generate the full report with integrated code, visualizations, and analyses.

## Key Insights
- **Variable Importance:** Key predictors such as gamma-GTP, hemoglobin, and age play a crucial role in predicting alcohol consumption.
- **Model Performance:** The optimized decision tree achieved an improved AUC-ROC (~0.75) over the basic model (~0.73), demonstrating enhanced discrimination between the classes.
- **Handling Missing Data:** Increasing levels of missing data notably degrade performance, underscoring the need for robust missing data techniques.
- **Future Directions:** Further improvements could involve ensemble methods to reduce overfitting and better handle data variability.

## Acknowledgements 🙏
Many thanks to the course instructors, peers, and mentors who provided support and guidance throughout this project.

Happy coding and data exploring! 🚀
