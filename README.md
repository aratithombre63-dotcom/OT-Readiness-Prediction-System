# 🏥 OT Readiness Prediction System

An intelligent **Operation Theatre (OT) Readiness Prediction System** designed to monitor operating theatre environmental conditions and predict whether an OT is ready for surgery.

The system uses Machine Learning to analyze environmental parameters and provides a dashboard to monitor OT conditions and readiness status.

## 📌 Project Overview

Operation Theatre readiness is important for maintaining a suitable environment before surgery. Several environmental parameters, such as temperature, humidity, air quality, pressure and airflow, need to be monitored.

This project aims to simplify OT monitoring by using a Machine Learning-based prediction system that analyzes environmental data and predicts OT readiness.

The application provides a dashboard for viewing environmental conditions and a control panel for updating input values.

## 🎯 Objectives

- Monitor important Operation Theatre environmental parameters.
- Predict OT readiness using Machine Learning.
- Display environmental information through a dashboard.
- Support different surgery types.
- Provide real-time-style monitoring through changing input values.
- Help users understand whether the OT environment meets configured readiness conditions.

## ✨ Key Features

- **OT Readiness Prediction:** Predicts the readiness status using a trained Machine Learning model.
- **Environmental Monitoring:** Monitors temperature, humidity, CO₂, PM2.5, PM10, TVOC and other parameters.
- **Interactive Dashboard:** Displays OT environmental information and prediction results.
- **Control Panel:** Allows users to update environmental values.
- **Surgery Type Selection:** Supports General Surgery, Cardiac Surgery, Neurosurgery and Orthopedic Surgery.
- **Live Data Updates:** Supports changing environmental values and updating predictions.
- **Bilingual Interface:** Includes English and Hindi language support.
- **Responsive Design:** Provides a user-friendly interface across different screen sizes.

## 🛠️ Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python, TypeScript, JavaScript |
| Machine Learning | Scikit-learn |
| Backend | Flask, Flask-CORS |
| Frontend | Angular, HTML, CSS |
| Data Processing | Pandas, NumPy |
| Model Handling | Joblib |
| Data Storage | CSV, JSON |
| Development Tools | VS Code, Git, GitHub |
| Package Management | npm, pip |

## 🧠 Machine Learning

The system uses a trained Machine Learning model to predict OT readiness based on environmental input parameters.

The project includes:

- Training dataset preparation
- Data generation and labeling
- Model training
- Feature importance analysis
- Readiness prediction
- Encoded categorical variables

The trained model and encoders are stored as `.pkl` files and used by the application for predictions.

## 📊 Environmental Parameters

The system monitors the following parameters:

- Temperature
- Humidity
- Differential Pressure
- Air Changes per Hour (ACH)
- Carbon Dioxide (CO₂)
- PM2.5
- PM10
- Total Volatile Organic Compounds (TVOC)
- Airflow Velocity
- Light Intensity
- Noise Level

## 🏗️ Project Structure

```text
OT-Readiness-Prediction-System/
│
├── frontend/                  # Angular frontend
│
├── templates/                 # HTML templates
│
├── app.py                     # Flask backend
├── control_panel.py           # OT control panel
│
├── model_training.py          # Model training
├── live_prediction.py         # Prediction functionality
├── feature_importance.py      # Feature importance
│
├── dataset_generator.py       # Dataset generation
├── dataset_generator_final.py
├── generate_labels.py         # Label generation
├── generate_training_dataset.py
│
├── ot_environment.csv         # Environmental data
├── training_dataset.csv       # Training dataset
│
├── ot_readiness_model.pkl     # Trained ML model
├── status_encoder.pkl         # Status encoder
├── surgery_encoder.pkl        # Surgery encoder
│
├── current_values.json        # Current OT values
├── current_index.txt
│
├── README.md
└── RUN_ME.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/aratithombre63-dotcom/OT-Readiness-Prediction-System.git
```

### 2. Open the Project Folder

```bash
cd OT-Readiness-Prediction-System
```

### 3. Install Python Dependencies

```bash
pip install flask flask-cors joblib pandas scikit-learn
```

### 4. Install Frontend Dependencies

```bash
cd frontend
npm install
cd ..
```

### 5. Start the Backend

Open the first terminal and run:

```bash
python app.py
```

Backend URL:

```text
http://127.0.0.1:5000
```

### 6. Start the Frontend

Open a second terminal:

```bash
cd frontend
npm start
```

Frontend URL:

```text
http://localhost:4200
```

### 7. Open the Application

Open your browser and visit:

```text
http://localhost:4200
```

**Requirements:**
- Python installed
- Node.js 20.19+ or 22.12+
- npm
- Git

## 🔄 Working Process

1. Environmental parameters are provided to the system.
2. The backend processes the input data.
3. The trained Machine Learning model analyzes the parameters.
4. The system generates an OT readiness prediction.
5. The frontend displays the environmental information and prediction results.
6. Users can update environmental values through the control panel.

## 🔮 Future Enhancements

- Integration with actual environmental sensors.
- Cloud-based data storage.
- Advanced prediction models.
- Automated alerts for unsuitable environmental conditions.
- Improved reporting and historical analysis.
- Deployment for practical testing in controlled environments.

## ⚠️ Disclaimer

This project is developed for academic and educational purposes. Its predictions are not a substitute for professional medical judgment, hospital protocols, or certified OT safety monitoring systems. The model and configured thresholds require proper validation before any real-world use.

## 👩‍💻 Author

**Arati Thombre**

B.Tech – Information Technology

GitHub: [@aratithombre63-dotcom](https://github.com/aratithombre63-dotcom)
