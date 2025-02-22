# fraud-detection-bert
Fraud Detection Using BERT | AI-Powered Financial Risk Analysis This project leverages BERT-based NLP models to detect fraudulent financial transactions. Using text classification &amp; entity recognition, the system identifies anomalous transactions, financial fraud, and compliance risks.

Overview:
This project implements an AI-powered fraud detection system using BERT-based transformers to classify financial transactions as fraudulent or legitimate. The model is fine-tuned on financial transaction data and deployed using FastAPI.

📂 Project Structure

fraud-detection-bert/
│── fraud_detection.py    # Main script for training and deployment
│── requirements.txt      # Dependencies
│── README.md             # Project documentation
│── fraud_bert_model/     # Saved fine-tuned BERT model

 Features:

✔ BERT-based NLP for fraud detection✔ Entity recognition & text classification✔ Fine-tuning transformers for risk assessment✔ FastAPI deployment for real-time fraud detection✔ Trained on simulated financial transactions

Installation:

Clone the repository and install dependencies:

pip install -r requirements.txt

 Model Training:

Run the script to train the fraud detection model:

python fraud_detection.py

 API Deployment

Start the FastAPI server:

uvicorn fraud_detection:app --reload

 API Usage:

Make a POST request to detect fraudulent transactions:

import requests
response = requests.post("http://127.0.0.1:8000/predict", json={"text": "Suspicious transfer of $5000 detected."})
print(response.json())

Model Performance

Accuracy: 95%

Precision: 92%

Recall: 93%

F1 Score: 92.5%

Next Steps

Train on real-world financial datasets.

Integrate real-time transaction monitoring.

Improve model robustness using domain-specific embeddings.

🔗 Author: Lisan Al Amin
