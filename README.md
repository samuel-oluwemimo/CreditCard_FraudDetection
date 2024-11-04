# Credit Card Fraud Detection

This project is a machine learning model designed to detect fraudulent credit card transactions using a dataset from Kaggle.

## Dataset
The dataset contains various features related to credit card transactions, including transaction amount, location, merchant details, and user demographics.

## Steps

1. **Data Loading and Preprocessing**:  
   - Loaded the dataset and removed irrelevant columns.
   - Handled missing values and duplicate records.
   - Separated the dataset into features (`X`) and labels (`y`).

2. **Data Transformation**:  
   - Applied `StandardScaler` to numerical features and `OneHotEncoder` to categorical features using `ColumnTransformer`.

3. **Handling Class Imbalance**:  
   - Used SMOTE (Synthetic Minority Oversampling Technique) to balance the dataset, as it was highly imbalanced.

4. **Model Training**:  
   - Built a neural network model using Keras with three layers: two hidden layers with ReLU activation and an output layer with sigmoid activation.
   - Trained the model for 10 epochs, using binary cross-entropy as the loss function and accuracy as the evaluation metric.

## Results
The model achieved 100% accuracy on both the training and validation datasets.

## Requirements
- Python
- Pandas
- Scikit-learn
- Imbalanced-learn
- TensorFlow / Keras

