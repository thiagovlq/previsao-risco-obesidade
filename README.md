Obesity Risk Prediction & Analysis
📌 Project Overview
This project was developed for a hospital environment to assist medical teams in predicting obesity risk levels. Using machine learning, the system classifies patients based on their physical condition and lifestyle habits.

📊 Business Context
Obesity is a multifactorial medical condition. The goal of this tool is to provide a data-driven approach for early diagnosis and personalized health recommendations.

🛠️ Technical Stack
Language: Python 3.13
Data Analysis: Pandas, NumPy, Matplotlib/Seaborn
Machine Learning: Scikit-Learn (Random Forest Classifier)
Deployment: Streamlit
Model Serialization: Joblib
📈 Key Results
Model Accuracy: 91.80% ✅
Dataset: 2,111 obesity records from UCI dataset
Classification Categories: 7 obesity levels (Insufficient Weight to Obesity Type III)
Best Performing Features: Weight, Height, Calorie monitoring, Physical activity frequency
Model Type: Random Forest (100 estimators)
🚀 How to Run
Quick Start (Recommended)
Double-click run_app.bat in the GitHub folder and the app will launch automatically.

Manual Setup
# 1. Create virtual environment
python -m venv venv

# 2. Activate it
venv\Scripts\Activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Navigate to project
cd obesity-risk-prediction

# 5. Train the model
python app/train.py

# 6. Run the app
python -m streamlit run app/app.py
The app will be available at http://localhost:8501

📁 Project Structure
obesity-risk-prediction/
├── app/
│   ├── app.py                    # Streamlit web application
│   ├── train.py                  # Model training script
│   └── model_pipeline.pkl        # Trained ML model
├── data/
│   ├── Obesity.csv               # Original dataset
│   └── processed_obesity.csv     # Processed dataset
├── notebook/
│   └── model_pipeline.ipynb      # Jupyter notebook with analysis
└── requirements.txt              # Python dependencies
🔧 Dependencies
See requirements.txt for the full list. Key packages:

scikit-learn==1.6.1
streamlit>=1.53.0
pandas>=1.4.0
numpy>=1.23
matplotlib & seaborn for visualization
