# 💼 Fraud Detection and Risk Assessment System

A robust and scalable machine learning system designed to detect fraudulent transactions in real-time using structured and unstructured data. This end-to-end project includes model training, sentiment-enhanced risk scoring, a live Flask API, an interactive dashboard, and a user-friendly web interface.

---

## 🔍 Features

- ✅ Machine Learning-based fraud detection using **Random Forest**
- 🧠 NLP integration with **Hugging Face Transformers** for unstructured data sentiment analysis
- ⚡ Real-time scoring via **Flask REST API**
- 📊 **Dash-powered dashboard** for data visualization and monitoring
- 🌐 Clean, responsive **frontend UI** (HTML + CSS)
- 📁 Modular code with proper **logging** and **exception handling**
- 📈 Achieved **AUC-ROC: 94.33%** on training data

---

## 🏗️ Project Structure

Fraud_Detection_Risk_Assessment/
│
├── api/ # Flask API for predictions
│ └── app.py
│
├── dashboard/ # Dash-based dashboard
│ └── app.py
│
├── data/ # Input datasets
│ └── transactions.csv
│
├── frontend/ # Web UI (HTML + CSS)
│ ├── index.html
│ └── style.css
│
├── logs/ # Logs for training & API
│
├── models/ # Trained model(s)
│ └── fraud_model.pkl
│
├── notebooks/ # Jupyter notebooks for EDA & modeling
│ └── EDA.ipynb
│
├── src/ # Source code for training
│ ├── train_model.py
│ ├── feature_engineering.py
│ └── utils.py
│
├── .gitignore
├── requirements.txt
└── README.md

yaml
Copy code

---

## 🚀 How to Run the Project

### 1. Clone the repository
```bash
git clone https://github.com/your-username/Fraud_Detection_Risk_Assessment.git
cd Fraud_Detection_Risk_Assessment
2. Install dependencies
bash
Copy code
pip install -r requirements.txt
3. Train the model (if model file isn't present)
bash
Copy code
python src/train_model.py
4. Run the Flask API
bash
Copy code
python api/app.py
Open browser at http://localhost:5000 for the UI.

5. Launch the Dashboard (Optional)
bash
Copy code
python dashboard/app.py
Open browser at http://127.0.0.1:8050 for visualizations.

🧠 Model Details
Algorithm: Random Forest Classifier

Metric: AUC-ROC = 94.33%

Data: Simulated or real transactional data (CSV format)

NLP: Hugging Face Transformers used for analyzing user remarks/comments if any

🛡️ Logging & Exception Handling
All API requests and model predictions are logged to /logs/

Graceful error handling for invalid input, model load errors, etc.

🌐 Frontend Preview
<!-- Optional: Add image here -->

📊 Sample Dashboard
Feature distributions

Fraud vs Non-Fraud visual trends

Model prediction probability histograms

📌 Future Improvements
Replace dummy sentiment with live transformer NLP model

Implement database persistence

Add role-based authentication for dashboard access

Deploy to cloud (Heroku, AWS, etc.)

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

📜 License
MIT

✨ Credits
Developed with ❤️ by [Your Name]