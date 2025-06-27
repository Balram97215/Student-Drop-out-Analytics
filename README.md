# Student-Drop-out-Analytics

Flag students at risk from dropping out of the program using predictive analytics.

---

## 📌 Project Overview

Student dropout, graduation, and continued enrollment represent significant educational outcomes that impact both individual futures and societal well-being. This project focuses on predicting whether students will **drop out** or **graduate**, allowing institutions to proactively support at-risk students.

We analyzed a dataset of **4424 records** with **35 demographic, academic, and socioeconomic features**, such as GPA, attendance rates, family income, and parental education.

---

## 📊 Features

- **Demographic**: age, gender, nationality, marital status, parental education, parental occupation  
- **Academic**: course, GPA, curricular units enrolled/approved, attendance type  
- **Socioeconomic**: family income, tuition fee status, scholarship holder  
- **Other**: special needs, debtor status, displaced status  

---

## 🛠️ Methods

- **EDA**: Visual and statistical exploration of categorical and numerical features  
- **Feature Engineering**: Aggregated academic performance features, removed low-impact features  
- **Models**: Random Forest, XGBoost, Voting Classifier (ensemble of the two)  
- **Simulations**: Explored dropout probability under controlled variations of key features (average grade, approved units, age)  

---

## 🔑 Key Results

- Final model (Voting Classifier with top 16 features):  
  - Balanced Accuracy: **0.93**  
  - F1 Score: **0.92**  
  - AUC: **0.96**

- **Top predictive features**:  
  - Average approved units  
  - Tuition fee payment status  
  - Average grade  
  - Average enrolled units  
  - Age at enrollment  

- **Insights**:  
  - Tuition status is the strongest dropout predictor (87% dropout among unpaid tuition students).  
  - Dropout risk decreases sharply when grades exceed 10 and approved units exceed 5 and 14.  
  - Older students and males have higher dropout risk.  

---

## 🚀 How to Use

1. Load the dataset (`dataset.csv`)  
2. Run the notebook (`Group13_Student Dropout_first_draft.ipynb`)  
3. The notebook guides through EDA, model training, evaluation, and simulations  

---

## 🏆 Conclusion

This model helps educational institutions identify students most at risk based on academic, financial, and demographic factors — enabling early intervention to reduce dropout rates.  

---

## 🤝 Contributors

- **Balram Iyengar** – Model design, simulations, feature importance  
- **Maneesh Rao** – EDA, preprocessing, XGBoost tuning  
- **Dhanush** – Feature selection, visualization, simulation analysis  

---

## 📚 References

- [Scikit-learn RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)  
- [XGBoost Documentation](https://xgboost.readthedocs.io/en/latest/python/python_api.html)  
- [Permutation Importance](https://scikit-learn.org/stable/modules/permutation_importance.html)  
- [VotingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.VotingClassifier.html)

---

