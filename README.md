# AI Capstone Project — Predicting Music Streaming Revenues

This capstone project demonstrates a complete end-to-end machine learning pipeline using Apache Spark, MLlib, and Flask. The goal is to predict future revenue based on country and date inputs for a music streaming service, following a real-world business use case.

---

## 📌 Project Features

- ✅ Revenue prediction using ALS (Alternating Least Squares) model
- ✅ Time-series based recommendations
- ✅ Flask API to serve real-time predictions
- ✅ Country-specific revenue forecasting
- ✅ Clean and modular project structure
- ✅ Tested with sample inputs

---

## 📁 Project Structure

capstone_project_complete/
├── flask_app/
│ ├── app.py # Flask application
│ ├── requirements.txt # Python dependencies
│ └── model/
│ └── model.pkl # Trained ALS model
├── spark_model/
│ ├── model_training.ipynb # Spark model training notebook
│ └── model_export.py # Code to save the trained model
└── README.md

yaml
Copy
Edit

---

## ⚙️ How to Run This Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/capstone_project_complete.git
cd capstone_project_complete
2. Set Up the Python Environment
bash
Copy
Edit
cd flask_app
pip install -r requirements.txt
3. Run the Flask App
bash
Copy
Edit
python app.py
The API will be available at:
📍 http://127.0.0.1:5000/predict

🧪 Example API Usage
Use any API testing tool like Postman or curl.

POST Request:
json
Copy
Edit
POST http://127.0.0.1:5000/predict
Content-Type: application/json

{
  "country": "India",
  "target_date": "2025-08"
}
Response:
json
Copy
Edit
{
  "country": "India",
  "target_date": "2025-08",
  "predicted_revenue": 43214.25
}
📊 Model Info
Framework: PySpark MLlib (ALS)

Model Type: Collaborative Filtering

Input: Country, Target Date

Output: Predicted Revenue

🛠️ Tech Stack
Apache Spark (PySpark)

Flask

Python

Pandas, Numpy

JSON API

✍️ Author
Divyesh Thakur
