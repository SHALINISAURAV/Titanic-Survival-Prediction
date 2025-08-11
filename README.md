# 🚢 Titanic Survival Prediction

Predict passenger survival from the Titanic disaster using **Machine Learning**.  
Trained with **Logistic Regression**, this model uses features like passenger class, age, sex, fare, and more.

## 🔹 Features
- Simple & clean implementation for beginners
- Data preprocessing & feature engineering
- Model saved as `titanic_model.pkl` for reuse
- import pickle, pandas as pd

with open('titanic_model.pkl', 'rb') as f:
    model = pickle.load(f)

sample = pd.DataFrame([[3, 1, 22, 1, 0, 7.25, 0]],
                      columns=['Pclass','Sex','Age','SibSp','Parch','Fare','Embarked'])
print("Survived" if model.predict(sample)[0] else "Not Survived")
