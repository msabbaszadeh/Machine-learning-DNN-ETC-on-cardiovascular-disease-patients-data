Cardiovascular Disease Prediction using AI and Machine Learning

This project applies Artificial Intelligence (AI) and Machine Learning (ML) techniques to predict the likelihood of cardiovascular diseases based on lifestyle, health indicators, and demographic data. The goal is to use data-driven insights to identify key risk factors and develop a predictive model that supports preventive healthcare decisions.

🧠 Project Overview

The dataset includes over 300,000 medical records with 19 health-related features such as BMI, age, alcohol consumption, exercise habits, diet, and chronic conditions.
Through data preprocessing, feature encoding, normalization, and model training, the project compares Deep Learning (Neural Networks) and Classical Machine Learning algorithms to evaluate which performs best in predicting heart-related conditions.

⚙️ Key Features

Comprehensive Data Analysis: Cleaned, balanced, and visualized a large-scale cardiovascular dataset.

Feature Engineering: Converted categorical data into numerical form using Label Encoding and manually defined mappings for ordered variables like Age and Health Status.

Data Normalization: Applied MinMaxScaler to improve model training stability and performance.

Model Comparison: Built and compared a Deep Neural Network (TensorFlow/Keras) and a Tree-Based Model (Extra Trees Classifier).

Feature Importance Analysis: Identified the most influential health and lifestyle factors contributing to cardiovascular disease risk.

Model Persistence: Saved the best-performing model using Joblib for future deployment.

🧩 Data Processing Workflow

Data Cleaning:

Removed duplicates and verified no missing values.

Balanced the dataset to ensure fair representation across classes.

Encoding:

Used Label Encoding to transform text attributes into numerical values.

Preserved logical order for features like Age Category and General Health.

Normalization:

Scaled all numerical features between 0 and 1 for optimal neural network performance.

Data Splitting:

Split into Training (75%) and Testing (25%) sets.

🤖 Model Development
Deep Learning Model (TensorFlow/Keras)

A fully connected neural network (Feed-Forward Neural Network) was designed with multiple dense layers using ReLU, SELU, and LeakyReLU activation functions.

Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Accuracy on Test Data: ~71%

Machine Learning Model (Extra Trees Classifier)

A tree-based ensemble algorithm was trained and evaluated on the same dataset for comparison.

Accuracy on Test Data: ~82%

Best Performing Model: Extra Trees Classifier

📊 Feature Importance Insights

The Extra Trees model provided interpretability through feature importance scores.
Top influencing factors associated with cardiovascular disease:

Green Vegetables Consumption 🥦

Fruit Consumption 🍎

Alcohol Consumption 🍷

Smoking History 🚬

Body Mass Index (BMI) ⚖️

Weight and Height

Age and Gender

These results emphasize that lifestyle choices—especially diet and alcohol use—have the strongest impact on cardiovascular health.

🩺 Results Summary
Model	Type	Test Accuracy	Key Strength
Deep Learning	Neural Network (Keras)	71.9%	Learns complex nonlinear patterns
Extra Trees Classifier	Ensemble ML	82.4%	High accuracy and feature interpretability
