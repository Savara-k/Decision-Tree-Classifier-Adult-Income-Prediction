# Decision-Tree-Classifier-Adult-Income-Prediction

UCI Adult Income Dataset Analysis
## Overview
This project implements and evaluates a Decision Tree Classifier to predict whether an individual’s annual income exceeds $50K based on demographic and employment attributes from the UCI Adult Income dataset.
The analysis addresses real-world machine learning challenges such as class imbalance, missing values, and categorical encoding, while exploring how model performance changes through parameter tuning and cross-validation.

## Objective
Predict income category:
* <=50K
* >50K
* using features such as:
* Age
* Education level
* Occupation
* Workclass
* Marital status
* Hours worked per week
* Capital gains/losses
* And more

---
## Dataset
UCI Adult Income Dataset
🔗 Kaggle:
https://www.kaggle.com/datasets/wenruliu/adult-income-dataset

Dataset Characteristics
* 48,842 records
* 14 demographic and employment attributes
* Binary classification target
Real-world issues:
* Class imbalance
* Missing values
* Categorical features

---
## Methodology
### Data Preprocessing
* Replaced missing values marked as ? with NaN
* Imputed missing values using the most frequent value
* Encoded categorical variables using Label Encoding
* Stratified train-test split (80/20)

### Model Development
Three Decision Tree configurations were evaluated:

- Default Decision Tree
* Accuracy: 81.48%
- Tuned Decision Tree
Parameters tested:
* max_depth = 5
* min_samples_split = 20
* criterion = entropy
* Accuracy improved to: 85.57%

---
## Evaluation Metrics
Classification performance assessed using:
* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
  
Key insight:
The tuned model significantly improved performance for the minority class (>50K), demonstrating the importance of hyperparameter optimization in imbalanced datasets.

---
## Decision Tree Visualization
The final model was visualized using:
* sklearn.tree.plot_tree
* (Optional) Graphviz for detailed visualization
Visualization helps interpret:
* Feature importance
* Decision rules
* Model transparency

---
## Tech Stack
* Python
* Pandas & NumPy — data processing
* Scikit-learn — machine learning
* Matplotlib & Seaborn — visualization
* KaggleHub — dataset access

---
## Key Takeaways
* Decision Trees provide interpretable models for classification tasks
* Hyperparameter tuning significantly improves performance
* Handling missing data and class imbalance is critical
* Model transparency makes Decision Trees valuable for real-world applications
