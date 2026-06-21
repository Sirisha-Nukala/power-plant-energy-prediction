# Power Plant Output Prediction using ANN

## Overview

This project uses an **Artificial Neural Network (ANN)** built with **PyTorch** to predict the **electrical energy output (PE)** of a combined cycle power plant. The model learns the relationship between environmental conditions and power generation to perform accurate regression-based predictions.

The project demonstrates a complete machine learning workflow, including:

* Data preprocessing
* Feature scaling
* Train-test splitting
* ANN model building
* Model training and validation
* Performance evaluation using regression metrics

---

## Dataset

The dataset contains power plant operational data with environmental variables as input features.

### Features

* **AT** — Ambient Temperature
* **V** — Exhaust Vacuum
* **AP** — Ambient Pressure
* **RH** — Relative Humidity

### Target Variable

* **PE** — Electrical Energy Output

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* PyTorch
* Matplotlib

---

## Project Workflow

### 1. Data Preprocessing

* Loaded dataset using Pandas
* Checked for missing values
* Separated features and target variable

### 2. Train-Test Split

* Training data: 80%
* Testing data: 20%

### 3. Feature Scaling

Used **StandardScaler** to normalize input features for better ANN performance.

### 4. Model Architecture

Implemented a feed-forward neural network with:

* Input layer: 4 neurons
* Hidden layer 1: 6 neurons + ReLU
* Hidden layer 2: 6 neurons + ReLU
* Output layer: 1 neuron

### 5. Training

* Loss Function: Mean Squared Error (MSE)
* Optimizer: Adam
* Epochs: 100
* Batch Size: 32

### 6. Evaluation

Model performance evaluated using:

* Mean Squared Error (MSE)
* R² Score

---

## Model Architecture

```python
Input Layer (4)
     ↓
Hidden Layer (6) + ReLU
     ↓
Hidden Layer (6) + ReLU
     ↓
Output Layer (1)
```

---

## Results

The ANN model successfully learned nonlinear relationships between environmental factors and energy output.

Evaluation metrics:

* Training MSE: *(Add your result here)*
* Testing MSE: *(Add your result here)*
* R² Score: *(Add your result here)*

---

## Loss Curve

Training and validation loss were plotted to monitor model performance and convergence across epochs.

---

## Key Learnings

Through this project, I gained practical experience in:

* Regression using Deep Learning
* Building neural networks in PyTorch
* Data preprocessing for ANN models
* Training and validating ML models
* Performance analysis using evaluation metrics

---

## Future Improvements

Possible enhancements:

* Hyperparameter tuning
* Deeper neural network architecture
* Cross-validation
* Experimenting with other regression models
* Deployment using Streamlit or Flask

---

## How to Run

1. Clone the repository

```bash
git clone <your-repository-link>
```

2. Install dependencies

```bash
pip install numpy pandas matplotlib scikit-learn torch
```

3. Run the notebook or Python script

---

## Author

**Sirisha Nukala**
Aspiring Data Analyst / Machine Learning Enthusiast
