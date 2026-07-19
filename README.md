# Customer Churn Prediction with Artificial Neural Networks

This project builds an end-to-end customer churn prediction system using an Artificial Neural Network (ANN) trained on a banking dataset. The trained model is exposed through a Streamlit web application that allows users to input customer details and receive a churn probability in real time.

## Project Overview

Customer churn prediction is a critical business use case in the banking and telecom industries. This project demonstrates how machine learning can be used to identify customers at risk of leaving a service, enabling proactive retention strategies.

The workflow includes:
- Data preprocessing and feature engineering
- Encoding categorical variables
- Feature scaling
- Training a neural network for binary classification
- Saving model artifacts for inference
- Building an interactive Streamlit app for predictions

## Technologies Used

- Python
- TensorFlow / Keras
- scikit-learn
- pandas
- NumPy
- Streamlit
- Jupyter Notebook

## Project Structure

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

## Dataset

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

## Model Summary

The ANN model is trained to predict whether a customer is likely to churn based on the given input features.

## How to Run Locally

1. Clone this repository:
   ```bash
   git clone <your-repository-url>
   cd ANN-CLASSIFICATION-End-to-End-Project
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```
   On Windows:
   ```bash
   venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## Usage

Once the app is running, enter the customer details in the sidebar or input fields and click through the app to obtain the churn prediction.

## Notes

- The model and preprocessing artifacts are already included in the repository for inference.
- This project is intended for learning and portfolio demonstration purposes.

## Future Improvements

Potential enhancements for this project include:
- Hyperparameter tuning
- Class imbalance handling
- Model explainability with SHAP or LIME
- Deploying the app on Streamlit Cloud, AWS, or Azure

## License

This project is intended for educational and portfolio purposes.
