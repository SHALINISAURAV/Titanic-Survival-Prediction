# 🚢 Titanic Survival Prediction  

Predict whether a passenger survived the Titanic disaster using **Machine Learning (Logistic Regression)**.  
This project is a beginner-friendly implementation that covers **data preprocessing, feature engineering, and model deployment** with a saved model file.  

---

## 📌 Project Overview  
The Titanic dataset is one of the most famous datasets in data science. It contains details about passengers such as **class, sex, age, fare, and family relations**.  
The goal is to build a model that predicts whether a passenger **survived (1)** or **not (0)**.  

---

## 🔹 Features  
- ✅ Clean & simple implementation (great for beginners)  
- ✅ Data preprocessing & feature engineering  
- ✅ Logistic Regression for classification  
- ✅ Model saved as **`titanic_model.pkl`** for reuse  
- ✅ Example prediction script included  

---

## 📂 Project Structure  
```
├── titanic_model.pkl        # Trained ML model
├── titanic_prediction.py    # Example script to test the model
├── README.md                # Project documentation
└── requirements.txt         # Dependencies
```

---

## 🛠️ Installation & Setup  

1. Clone the repository:
   ```bash
   git clone https://github.com/SHALINISAURAV/titanic-survival-prediction.git
   cd titanic-survival-prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the sample prediction:
   ```bash
   python titanic_prediction.py
   ```

---

## 📊 Example Usage  

```python
import pickle, pandas as pd

# Load trained model
with open('titanic_model.pkl', 'rb') as f:
    model = pickle.load(f)

# Sample passenger: [Pclass, Sex, Age, SibSp, Parch, Fare, Embarked]
sample = pd.DataFrame(
    [[3, 1, 22, 1, 0, 7.25, 0]],
    columns=['Pclass','Sex','Age','SibSp','Parch','Fare','Embarked']
)

print("✅ Survived" if model.predict(sample)[0] else "❌ Not Survived")
```

**Output Example:**
```
❌ Not Survived
```

---

## 📈 Model Performance  
- Algorithm: **Logistic Regression**  
- Accuracy: ~80% (depending on preprocessing)  
- Evaluation Metric: Accuracy Score  

---

## 🚀 Future Improvements  
- Try advanced models (Random Forest, XGBoost, Neural Networks)  
- Perform hyperparameter tuning  
- Use cross-validation for better generalization  
- Deploy using **Streamlit** or **Flask** for a web interface  

---

## 👩‍💻Author✨ 
**Your Name**  
📧 [shalinisourav07@gmail.com]  
🌐 [https://github.com/SHALINISAURAV]  

---

✨ *A classic beginner-friendly ML project to kickstart your Data Science journey!*  
