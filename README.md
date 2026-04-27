🔬 MAGIC Gamma Telescope Classification Project
📌 Overview

This project applies multiple machine learning classification models to the MAGIC Gamma Telescope dataset, which simulates the detection of high-energy gamma particles using atmospheric Cherenkov imaging.

The dataset contains two classes:

Gamma (signal)
Hadron (background)

The main goal is to build, tune, and evaluate different classifiers and compare their performance.

🎯 Objectives
Explore different classification models
Handle class imbalance in the dataset
Tune hyperparameters using cross-validation
Evaluate models using multiple metrics
Visualize results using confusion matrices and accuracy comparison
📊 Dataset
Source: MAGIC Gamma Telescope dataset
Total samples:
Gamma: 12332
Hadron: 6688
Features:

10 continuous numerical features describing event characteristics:

fLength
fWidth
fSize
fConc
fConc1
fAsym
fM3Long
fM3Trans
fAlpha
fDist
⚙️ Preprocessing
Removed duplicates (if any)
Balanced dataset using undersampling
Encoded target labels (g → 1, h → 0)
Split data into:
70% training
30% testing (stratified)
🤖 Models Used

The following classification models were implemented:

🌳 Decision Tree
🚀 AdaBoost (with hyperparameter tuning)
🌲 Random Forest (with GridSearchCV tuning)
🧠 Naive Bayes
🔧 Hyperparameter Tuning

Used GridSearchCV with 5-fold cross validation for:

AdaBoost → n_estimators
Random Forest → n_estimators
📈 Evaluation Metrics

Each model was evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
📊 Visualization
Confusion Matrix Heatmaps for each model
Accuracy comparison bar chart
Feature importance (Random Forest)
🏆 Results Summary

The models achieved strong performance:

Accuracy reached ~96% in best models
Random Forest and AdaBoost showed strong performance compared to others
Balanced dataset improved fairness between classes
🛠️ Technologies Used
Python 🐍
Pandas
NumPy
Scikit-learn

💡 Key Insights
Balancing the dataset significantly improved model fairness
Ensemble methods (Random Forest & AdaBoost) outperformed single models
Cross-validation helped in selecting optimal hyperparameters
📌 Author

Fady Anton
Machine Learning Project – Classification Lab
Matplotlib
Seaborn
