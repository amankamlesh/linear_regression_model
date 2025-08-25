🔥 Algerian Fire Weather Index (FWI) Prediction

📌 Project Overview

This project predicts the Fire Weather Index (FWI) using the Algerian Forest Fires Dataset.
FWI is an important indicator for wildfire risk assessment, helping authorities estimate the likelihood and severity of forest fires.

The solution involves:

Exploratory Data Analysis (EDA) and preprocessing

Feature scaling and transformation

Training a Ridge Regression model

Deploying a Flask web application on Render

📊 Dataset

Name: Algerian Forest Fires Dataset

Files Included:

Algerian_forest_fires_cleaned_data.csv

Algerian_forest_fires_dataset_UPDATED.csv

Features:

Temperature, Relative Humidity, Wind Speed, Rain

FFMC, DMC, DC, ISI, BUI

Classes, Region

Target: Fire Weather Index (FWI)

Source: UCI Repository – Algerian Forest Fires Dataset

⚙️ Tech Stack

Python 3.x

Flask (backend framework)

HTML/CSS (frontend templates)

scikit-learn (Ridge Regression model + preprocessing)

pandas / numpy / matplotlib

Render (deployment)

AWS Elastic Beanstalk configs (.ebextensions/)

🚀 How to Run Locally
1️⃣ Clone the repository
git clone https://github.com/amankamlesh/linear_regression_model.git
cd linear_regression_model

2️⃣ Create a virtual environment
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

3️⃣ Install dependencies
pip install -r requirement.txt

4️⃣ Run the Flask app
python application.py


The app will be available at:
👉 http://127.0.0.1:5000/predictdata

🌐 Deployment

The project is deployed on Render and can be accessed here:
👉 [Live Demo](https://fire-weather-index-6zze.onrender.com/predictdata)

It also includes AWS Elastic Beanstalk configuration files (.ebextensions/) for cloud deployment.

📈 Results

Model Used: Ridge Regression

Evaluation Metric: R² Score (0.984)

Example:

Ridge Regression achieved an R² score of 0.89 on the test dataset, showing reliable performance in predicting FWI.

📂 Project Structure
linear_regression_model/
├── .ebextensions/                     # AWS Elastic Beanstalk configs
├── EDA and model training/            # Notebooks & scripts for analysis
├── models/                            # (Optional) model storage
├── templates/                         # HTML templates for Flask app
├── Algerian_forest_fires_cleaned_data.csv
├── Algerian_forest_fires_dataset_UPDATED.csv
├── application.py                     # Flask application entry point
├── requirement.txt                    # Python dependencies
├── ridge.pkl                          # Trained Ridge Regression model
├── scaler.pkl                         # Fitted Scaler object
└── README.md                          # Project documentation

✨ Future Improvements

Compare Ridge Regression with other models (Random Forest, XGBoost, Neural Networks)

Add risk categorization (Low, Medium, High fire risk) instead of raw FWI values

Integrate real-time weather API for live predictions

Enhance UI with better visualization

👨‍💻 Author

Aman Kamlesh Mahor

GitHub: @amankamlesh

LinkedIn: [https://www.linkedin.com/in/aman-mahor-4589a6229/]
