# Survival Prediction 🛳️

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-0.25-orange?logo=scikitlearn)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone on board, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).
This project predicts survival outcomes of passengers using machine learning. The goal is to classify whether a passenger survived or not based on demographic and travel information.

---

## 📊 Dataset

The dataset contains passenger information such as age, sex, class, and family relationships.  

**Sample columns:**

| Feature       | Description                                      |
|---------------|--------------------------------------------------|
| PassengerId   | Unique ID of each passenger                     |
| Pclass        | Passenger class (1st, 2nd, 3rd)                 |
| Name          | Passenger name                                  |
| Sex           | Gender                                          |
| Age           | Age in years                                    |
| SibSp         | Number of siblings/spouses aboard               |
| Parch         | Number of parents/children aboard               |
| Ticket        | Ticket number                                   |
| Fare          | Passenger fare                                  |
| Cabin         | Cabin number                                    |
| Embarked      | Port of Embarkation (C, Q, S)                  |

---

## 🔄 Data Preprocessing

- Handle missing values for `Age`, `Cabin`, and `Embarked`.
- Encode categorical variables (`Sex`, `Embarked`) using label encoding or one-hot encoding.
- Scale numerical features when necessary.
- Split dataset into training and testing sets.

---

## 🤖 Modeling

**Gradient Boosting Classifier** was used for prediction.  

**Hyperparameters:**
- `learning_rate = 0.001`
- `max_depth = 3`
- `n_estimators = 500`
- `min_samples_split = 5`
- `min_samples_leaf = 3`
- `random_state = 42`

Other models tested: Decision Trees, Random Forest, SVM.

---

## 📈 Evaluation

Performance metrics:

| Metric     | Score |
|------------|-------|
| Accuracy   | 0.79  |
| Precision  | 0.86  |
| Recall     | 0.55  |
| F1-Score   | 0.67  |

---

## 🏆 Results

- Model can predict survival with ~79% accuracy.
- High precision indicates most predicted survivors were correct.
- Recall is moderate; some actual survivors are missed.
- Feature importance highlights `Sex`, `Pclass`, and `Age` as most influential.

---

**Confusion Matrix:**

![Confusion Matrix](confusion_matrix.png)

---

## 👨‍💻 Author

**Aldous Dsouza**  
BSc Computer Science Graduate | Data Science Enthusiast  


