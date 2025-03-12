ML Intern Task - Hyperspectral Imaging for Mycotoxin Prediction

 This project processes hyperspectral imaging data, applies dimensionality reduction, and trains a machine learning model to predict mycotoxin (DON) levels in corn samples.

 MLtask/
│── data/                   # Raw & processed data
│   ├── data.csv            # Original dataset (provided)
│   ├── processed_data.csv   # Preprocessed dataset
│
│── models/                 # Trained models
│   ├── trained_model.pkl    # Saved ML model
│
│── results/                # Evaluation results
│   ├── evaluation_metrics.csv  # Model performance metrics
│
│── src/                    # Source code
│   ├── data_exploration.py  # EDA & visualization
│   ├── preprocessing.py     # Data cleaning & normalization
│   ├── dim_reduction.py     # PCA & t-SNE for dimensionality reduction
│   ├── train_model.py       # ML model training
│   ├── evaluate_model.py    # Model evaluation
│
│── report.md                # Short report with findings
│── README.md                # Project instructions
│── requirements.txt         # Required Python dependencies
│── .gitignore               # Ignore unnecessary files


Objective
This project focuses on predicting mycotoxin levels in corn samples using hyperspectral imaging data by:
✔ Preprocessing spectral reflectance data
✔ Applying PCA/t-SNE for dimensionality reduction
✔ Training a regression model (XGBoost/Random Forest)
✔ Evaluating model performance with MAE, RMSE, and R² Score

Setup & Installation
1️⃣ Clone the Repository
git clone https://github.com/yashwanth-208/Ml_intern_task
cd ML-Intern-Task

2️⃣ Create a Virtual Environment (Recommended)
## 🛠️ Setup
After cloning, install dependencies:
```sh
python -m venv venv 
venv\Scripts\activate     # Windows
pip install -r requirements.txt

Usage
1️⃣ Preprocess the Data
python src/preprocessing.py

2️⃣ Train the Model
python src/train_model.py

3️⃣ Evaluate the Model
python src/evaluate_model.py

📈 Results
The trained model achieved:
✔ Mean Absolute Error (MAE): 3410.23
✔ Root Mean Squared Error (RMSE): 13519.86
✔ R² Score: -0.0679 (Indicates model needs improvements)
