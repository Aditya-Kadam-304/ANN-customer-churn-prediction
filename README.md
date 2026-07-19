# Customer Churn Prediction with Artificial Neural Networks

[![Streamlit App](https://img.shields.io/badge/Streamlit-App-FF4B4B?logo=streamlit&logoColor=white)](https://streamlit.io)

This project builds an end-to-end customer churn prediction system using an Artificial Neural Network (ANN) trained on a banking dataset. The trained model is deployed through a Streamlit web application that allows users to input customer details and receive a churn probability in real time.

## 🔗 Live Application

The public Streamlit deployment link will appear here once the app is published on Streamlit Community Cloud.

For now, the app can be run locally with:
```bash
streamlit run app.py
```

## Project Overview

Customer churn prediction is a critical business use case in the banking and telecom industries. This project demonstrates how machine learning can be used to identify customers at risk of leaving a service, enabling proactive retention strategies.

The workflow includes:
- Data preprocessing and feature engineering
- Encoding categorical variables
- Feature scaling
- Training a neural network for binary classification
- Saving model artifacts for inference
- Building an interactive Streamlit app for predictions

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- scikit-learn
- pandas
- NumPy
- Streamlit
- Jupyter Notebook

## 📁 Project Structure

```text
.
├── app.py                      # Streamlit web application
├── Churn_Modelling.csv        # Dataset used for training
├── model.h5                   # Trained ANN model
├── scaler.pkl                 # Feature scaler
├── label_encoder_gender.pkl   # Gender encoder
├── onehot_encoder_geo.pkl     # Geography encoder
├── experiments.ipynb          # Experimentation and training notebook
├── predictions.ipynb          # Prediction workflow notebook
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
```

## 📊 Dataset

The project uses a customer churn dataset containing features such as:
- Credit Score
- Geography
- Gender
- Age
- Tenure
- Balance
- Number of Products
- Credit Card status
- Active member status
- Estimated Salary

## 🧠 Model Architecture

The model uses a multi-layer deep learning structure built with the Keras Sequential API:
- Input layer matching the preprocessed feature vectors
- Dense hidden layers with ReLU activation
- Output layer with a Sigmoid activation to predict churn probability
- Loss function: Binary Crossentropy
- Optimizer: Adam

## ▶️ How to Run Locally

1. Clone this repository:
   ```bash
   git clone <your-repository-url>
   cd ANN-CLASSIFICATION-End-to-End-Project
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   ```
   On Windows:
   ```bash
   venv\Scripts\activate
   ```
   On macOS/Linux:
   ```bash
   source venv/bin/activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## 🚀 Usage

Once the application loads, use the input panel to adjust the customer attributes such as Age, Credit Score, Balance, and Geography. The model processes the inputs and returns a live probability indicating whether the customer is likely to churn.

## 🔮 Future Improvements

Potential enhancements for this project include:
- Hyperparameter tuning using Keras Tuner
- Class imbalance handling with techniques such as SMOTE
- Model explainability with SHAP or LIME
- Deployment improvements for cloud-based production environments

## 📄 License

This project is intended for educational and portfolio purposes.
