# 🧠 Artificial Neural Network (ANN) for Customer Churn Prediction

This project builds and trains an **Artificial Neural Network (ANN)** to predict whether a customer will leave a bank, using structured data and deep learning techniques.

---

## 📂 Dataset

We use the `Churn_Modelling.csv` dataset, which contains information on 10,000 bank customers. The goal is to predict the binary target variable:  
**Exited** – whether the customer left the bank (1) or not (0).

---

## 🛠️ Project Structure

### 1. Data Preprocessing

- **Load Dataset**  
  Read the dataset and extract the independent variables `X` and target variable `y`.

- **Encode Categorical Data**  
  - `Gender`: Label Encoding  
  - `Geography`: One Hot Encoding (with ColumnTransformer)

- **Split Dataset**  
  80% Training / 20% Testing split using `train_test_split`.

- **Feature Scaling**  
  Normalize input features using `StandardScaler`.

### 2. Building the ANN

- **Model Architecture**  
  - Input layer  
  - 2 Hidden layers (6 neurons each, ReLU activation)  
  - Output layer (1 neuron, Sigmoid activation for binary classification)

### 3. Training the ANN

- **Compile the Model**  
  - Optimizer: `adam`  
  - Loss: `binary_crossentropy`  
  - Metrics: `accuracy`

- **Fit the Model**  
  Train on the training set for `100 epochs` with batch size `32`.

### 4. Evaluation & Prediction

- **Single Observation Prediction**  
  Predict whether a given customer with specified features would churn.

- **Test Set Prediction**  
  Compare predictions with ground truth and evaluate performance using:
  - Confusion Matrix
  - Accuracy Score

---

## 🧪 Sample Prediction

**Customer Info**  
