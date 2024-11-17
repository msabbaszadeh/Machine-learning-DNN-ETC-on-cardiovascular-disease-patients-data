Features of the Project

    Data Analysis:
        Data cleaning and preprocessing.
        Statistical analysis and hypothesis testing.
    Data Visualization:
        Correlation heatmaps.
        Distribution plots for variables.
        Comparative analysis through bar plots and scatter plots.
    Deep Learning Model:
        Constructed using TensorFlow and Keras.
        Incorporates advanced activation functions like LeakyReLU, SELU, and ReLU.
        Includes an early stopping mechanism to avoid overfitting.
    Feature Importance Ranking:
        Insights into the most influential factors contributing to CVD.

Technologies Used

    Programming Language: Python
    Libraries and Frameworks:
        Pandas
        NumPy
        Matplotlib
        Seaborn
        TensorFlow/Keras

Deep Learning Model Details
Model Architecture

    Input Layer: Features from the dataset.
    Hidden Layers:
        Four dense layers with varying activation functions (LeakyReLU, SELU, and ReLU).
        Additional dense layers with a focus on increased capacity (400 and 30 neurons).
    Output Layer: Two neurons with a softmax activation function for binary classification.

DL_model = tf.keras.Sequential([
    tf.keras.layers.Dense(hidden_layer_size, activation='LeakyReLU'),
    tf.keras.layers.Dense(hidden_layer_size, activation='selu'),
    tf.keras.layers.Dense(hidden_layer_size, activation='relu'),
    tf.keras.layers.Dense(hidden_layer_size, activation='relu'),
    tf.keras.layers.Dense(400, activation='relu'),
    tf.keras.layers.Dense(30, activation='selu'),
    tf.keras.layers.Dense(output_size, activation='softmax')
])
DL_model.compile(optimizer='adam', loss='sparse_categorical_crossentropy', metrics=['accuracy'])

Training Details

    Batch Size: 175
    Epochs: 30 (early stopping after 6 epochs if no improvement).
    Optimizer: Adam
    Loss Function: Sparse Categorical Crossentropy
    Evaluation Metric: Accuracy



    EDA Highlights

    Demographic and Lifestyle Factors: Explored age, gender, dietary habits, physical activity, and medical history.
    Correlations: Strong associations identified between certain features (e.g., diet, exercise) and cardiovascular disease.
    Visualizations:
        Correlation heatmaps revealed dependencies among variables.
        Comparative bar plots emphasized the impact of green vegetable and fruit consumption on CVD risk.


Key Findings

    Lifestyle Factors Matter:
        Eating green vegetables and fruits is the most significant feature in reducing the risk of CVD.
        Other important factors include physical activity, smoking status, and BMI.
    Predictive Power:
        The deep learning model achieved high accuracy in predicting CVD presence.


Conclusion

This project emphasizes the importance of data-driven insights and advanced modeling techniques in understanding and predicting cardiovascular disease. 
The analysis highlights actionable lifestyle changes, like increased consumption of green vegetables and fruits, to mitigate CVD risk.

For further improvements, additional features or more complex neural network architectures could be explored to refine predictions.
