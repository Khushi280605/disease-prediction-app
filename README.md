# 🏥 Multi-Disease Prediction System

A Machine Learning based web application that predicts multiple diseases using medical parameters.  
The system integrates multiple trained ML models into a single Streamlit interface for real-time predictions.



## 📌 Project Overview

This project was built to understand and implement the complete Machine Learning workflow:

- Data Collection  
- Data Preprocessing  
- Feature Selection  
- Model Training  
- Model Evaluation  
- Model Serialization  
- Deployment using Streamlit  

The application currently predicts the following diseases:

- Diabetes
- Heart Disease
- Parkinson’s Disease
- Lung Cancer
- Thyroid Disorder



## 🧠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Streamlit
- Pickle



## 🔄 Machine Learning Pipeline

1. Load dataset  
2. Perform preprocessing  
   - Handle missing values  
   - Encode categorical variables  
   - Remove irrelevant features  
3. Split data (80% Training / 20% Testing)  
4. Train model  
5. Evaluate model performance  
6. Save trained model using Pickle  
7. Integrate into Streamlit web app  



# 📊 Model Details & Accuracy

## 1️⃣ Heart Disease Prediction

**Algorithm Used:** Logistic Regression  
**Number of Features:** 13  

### Features Used:
- age  
- sex  
- cp  
- trestbps  
- chol  
- fbs  
- restecg  
- thalach  
- exang  
- oldpeak  
- slope  
- ca  
- thal  

### Accuracy:
- Training Accuracy: **85.1%**
- Test Accuracy: **81.9%**



## 2️⃣ Lung Cancer Prediction

**Algorithm Used:** Logistic Regression  
**Number of Features:** 15  

### Features Used:
- GENDER  
- AGE  
- SMOKING  
- YELLOW_FINGERS  
- ANXIETY  
- PEER_PRESSURE  
- CHRONIC_DISEASE  
- FATIGUE  
- ALLERGY  
- WHEEZING  
- ALCOHOL_CONSUMING  
- COUGHING  
- SHORTNESS_OF_BREATH  
- SWALLOWING_DIFFICULTY  
- CHEST_PAIN  

### Accuracy:
- Training Accuracy: **93.5%**
- Test Accuracy: **93.5%**



## 3️⃣ Parkinson’s Disease Detection

**Algorithm Used:** Support Vector Machine (Linear Kernel)  
**Number of Features:** 22  

### Features Used:
- MDVP:Fo(Hz)  
- MDVP:Fhi(Hz)  
- MDVP:Flo(Hz)  
- MDVP:Jitter(%)  
- MDVP:Jitter(Abs)  
- MDVP:RAP  
- MDVP:PPQ  
- Jitter:DDP  
- MDVP:Shimmer  
- MDVP:Shimmer(dB)  
- Shimmer:APQ3  
- Shimmer:APQ5  
- MDVP:APQ  
- Shimmer:DDA  
- NHR  
- HNR  
- RPDE  
- DFA  
- spread1  
- spread2  
- D2  
- PPE  

### Accuracy:
- Training Accuracy: **87.1%**
- Test Accuracy: **87.1%**



## 4️⃣ Thyroid Disease Prediction

**Algorithm Used:** Logistic Regression  
**Number of Final Features After Preprocessing:** 7  

### Features Used:
- age  
- sex  
- on thyroxine  
- TSH  
- T3  
- TT4  
- FTI  

### Accuracy:
- Training Accuracy: **95.6**
- Test Accuracy: **95.6%**



## 5️⃣ Diabetes Prediction

**Algorithm Used:** Logistic Regression  
**Number of Features:** 8  

### Features Used:
- Pregnancies  
- Glucose  
- BloodPressure  
- SkinThickness  
- Insulin  
- BMI  
- DiabetesPedigreeFunction  
- Age  

### Accuracy:
- Test Accuracy: Model achieved strong predictive performance on test data.



# 💻 Web Application (Streamlit)

The web application allows users to:

1. Select a disease from the dropdown menu  
2. Enter relevant medical parameters  
3. Click the prediction button  
4. Get real-time prediction results  

Models are loaded dynamically using Pickle without retraining.



## 📁 Project Structure

```
multi-disease-prediction-app
│
├── app.py
├── Models
│   ├── diabetes_model.sav
│   ├── heart_disease_model.sav
│   ├── parkinsons_model.sav
│   ├── lungs_disease_model.sav
│   └── Thyroid_model.sav
│
├── requirements.txt
└── README.md
```



## ▶️ How to Run the Project

1. Clone the repository

```
git clone https://github.com/Khushi280605/disease-prediction-app
cd disease-prediction-app
```

2. Install dependencies

```
pip install -r requirements.txt
```

3. Run the Streamlit app

```
streamlit run app.py
```



# 🚀 Future Improvements

- Use larger and more diverse medical datasets  
- Experiment with ensemble models (Random Forest, Gradient Boosting)  
- Add cross-validation  
- Deploy on cloud platforms (AWS / Streamlit Cloud)  
- Add more diseases  



# 📚 Learning Outcome

This project helped in understanding:

- End-to-end Machine Learning workflow  
- Data preprocessing techniques  
- Model training and evaluation  
- Model deployment using Streamlit  
- Integration of multiple ML models into one system  
