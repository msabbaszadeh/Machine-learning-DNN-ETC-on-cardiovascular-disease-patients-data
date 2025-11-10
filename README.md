---

# 🫀 **Cardiovascular Disease Prediction using AI and Machine Learning**

This project leverages **Artificial Intelligence (AI)** and **Machine Learning (ML)** techniques to predict the likelihood of **cardiovascular diseases** based on lifestyle habits, medical history, and demographic data.
The goal is to use **data-driven insights** to identify key health risk factors and build a **predictive model** for early prevention and better healthcare decisions.

---

## 🧠 **Project Overview**

The dataset includes over **300,000 medical records** with **19 features**, covering health indicators such as **BMI, Alcohol Consumption, Smoking History, Exercise Habits, Diet, and Age**.

Through extensive **data cleaning**, **feature encoding**, **normalization**, and **model comparison**, the project evaluates both **Deep Learning (Neural Networks)** and **Classical Machine Learning (Extra Trees Classifier)** to determine the most effective prediction method.

---

## ⚙️ **Key Features**

* **Comprehensive Data Processing** — cleaning, balancing, and visualizing a large-scale health dataset.
* **Feature Encoding** — transformed categorical data into numerical form using **Label Encoding** and logical mappings.
* **Normalization** — applied **MinMaxScaler** for better training performance and model convergence.
* **Model Comparison** — evaluated a **Deep Neural Network (TensorFlow/Keras)** vs. **Extra Trees Classifier (Sklearn)**.
* **Feature Importance Analysis** — identified which health and lifestyle features most strongly influence cardiovascular risks.
* **Model Persistence** — saved the best-performing model as a **`.pkl` file** for deployment.

---

## 🧩 **Data Processing Workflow**

1. **Data Cleaning**

   * Removed duplicates (80 entries).
   * Verified there were **no missing values**.
   * Balanced target classes to ensure fair training.

2. **Encoding**

   * Applied **Label Encoding** for categorical features.
   * Maintained **logical order** for features like *Age Category* and *General Health*.

3. **Normalization**

   * Used **MinMaxScaler** to scale values between 0 and 1.

4. **Data Splitting**

   * **Training Set:** 75%
   * **Testing Set:** 25%

---

## 🤖 **Model Development**

### 🧬 **Deep Learning Model (TensorFlow/Keras)**

* **Architecture:** Multi-layer feed-forward neural network (Dense Layers)
* **Activations:** LeakyReLU, SELU, ReLU
* **Optimizer:** Adam
* **Loss Function:** Sparse Categorical Crossentropy
* **Early Stopping:** Enabled to prevent overfitting
* **Test Accuracy:** **≈ 71.9%**

---

### 🌲 **Machine Learning Model (Extra Trees Classifier)**

* **Algorithm:** Ensemble Tree-Based Classifier
* **Advantages:** Fast, interpretable, robust to noise
* **Test Accuracy:** **≈ 82.4%**
* **Best Performing Model:** ✅ **Extra Trees Classifier**

---

## 📊 **Feature Importance Analysis**

The **Extra Trees Classifier** identified which features contribute most to predicting **cardiovascular disease risk**:

| Rank | Feature                          | Importance |
| ---- | -------------------------------- | ---------- |
| 🥇 1 | **Green_Vegetables_Consumption** | **0.1733** |
| 🥈 2 | **Fruit_Consumption**            | **0.1022** |
| 🥉 3 | **Alcohol_Consumption**          | **0.0968** |
| 4    | Smoking_History                  | 0.0874     |
| 5    | BMI                              | 0.0872     |
| 6    | Weight_(kg)                      | 0.0872     |
| 7    | Height_(cm)                      | 0.0817     |
| 8    | Age_Category                     | 0.0733     |
| 9    | Sex                              | 0.0608     |
| 10   | Arthritis                        | 0.0304     |

🩺 **Insight:** Lifestyle factors such as **diet**, **alcohol intake**, and **smoking habits** are the most critical predictors of cardiovascular disease.

---

## 🧾 **Results Summary**

| **Model**              | **Type**               | **Test Accuracy** | **Key Strength**                         |
| ---------------------- | ---------------------- | ----------------- | ---------------------------------------- |
| Deep Learning          | Neural Network (Keras) | **71.9%**         | Learns complex nonlinear health patterns |
| Extra Trees Classifier | Ensemble ML            | **82.4% ✅**       | Higher accuracy and interpretability     |

**✅ The Extra Trees Classifier outperformed the Deep Neural Network by ~10%.**
This demonstrates that **classical ML models** can be more effective for structured health data than deep learning.

---

## 💾 **Model Deployment**

The best-performing model was saved for future use:

* **File Name:** `model.pkl`
* **Format:** Joblib serialized model
* **Use Case:** Ready for real-time predictions, healthcare dashboards, or clinical AI systems

---

## 🔍 **Related Keywords**

**AI in Healthcare**, **Machine Learning for Heart Disease**, **Cardiovascular Disease Prediction**, **Deep Learning Health Analytics**, **Feature Importance Analysis**, **Preventive Health AI**, **TensorFlow Classification Model**, **Medical Data Science Project**, **Python Machine Learning**, **Healthcare Predictive Modeling**, **AI for Public Health**, **Cardio Risk Prediction with ML**

---

## 👨‍💻 **Author**

**Developed by:** *Mohammad Sadegh Abbaszadeh*
💼 *Data Scientist | AI & Machine Learning Enthusiast*
🔗 GitHub: [github.com/msabbaszadeh](https://github.com/msabbaszadeh)
💬 *"Stay healthy, eat greens, avoid alcohol — the data proves it!"*

---

## 🧩 **Conclusion**

**✅ Final Insights:**

* The **Extra Trees Classifier** achieved **82.4% accuracy**, outperforming the neural network.
* **Lifestyle choices** — such as **diet**, **alcohol consumption**, and **smoking** — are **the most influential factors** in predicting cardiovascular disease.
* **Machine Learning can effectively predict health risks** and provide actionable insights for preventive healthcare.
* **Healthy habits = Lower heart disease risk.**

---
