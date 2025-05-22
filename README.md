# Titanic - Machine Learning from Disaster

This project is a solution to the **Kaggle Titanic: Machine Learning from Disaster** competition, one of the most popular beginner-friendly challenges for data science and machine learning enthusiasts. It aims to predict which passengers survived the Titanic shipwreck using classification techniques based on passenger data like age, sex, ticket class, etc.



##  Objective

The challenge is to **build a predictive model** that answers the question:

> *“What sorts of people were more likely to survive?”*

Using data such as:

* Name
* Age
* Sex
* Socio-economic class (ticket class)
* Fare
* Embarkation port


##  Dataset Overview

The dataset provided by Kaggle contains three CSV files:

1. **train.csv** – Contains data for 891 passengers, including the target variable `Survived` (1 = survived, 0 = did not survive).
2. **test.csv** – Contains data for 418 passengers without the `Survived` column. This is used for model predictions.
3. **gender\_submission.csv** – A sample submission assuming all females survived and males didn’t. This file demonstrates the required format for submission.



##  Data Preprocessing

### Training Data:

* Filled missing values (e.g., age, embarked).
* Encoded categorical variables (e.g., `Sex`, `Embarked`) using label encoding or one-hot encoding.
* Dropped unnecessary columns like `Name`, `Ticket`, and `Cabin` which may not add predictive power.
* Separated features (`X`) and target (`y`) from the training data.

### Testing Data:

* Applied the same preprocessing steps as training data.
* Ensured consistent feature structure for prediction.

---

##  Model Training – Random Forest Classifier

Steps involved in model building:

1. **Train-Test Split**: Divided the dataset into training and validation sets.
2. **Model Selection**: Used `RandomForestClassifier` from `sklearn` due to its robustness and interpretability.
3. **Training**: Fit the model on the training set.
4. **Evaluation**: Predicted on validation data and measured accuracy.
5. **Final Predictions**: Made predictions on the preprocessed `test.csv`.



##  Model Performance

* The Random Forest model was evaluated using accuracy on the validation set.
* Final predictions were submitted to Kaggle for scoring.



##  Submission

* Predictions on the test data were formatted as per the sample file: `PassengerId`, `Survived`.
* The submission was uploaded on Kaggle, and the leaderboard score was recorded.



##  Technologies Used

* **Python**
* **Pandas**
* **Scikit-learn**
* **Matplotlib / Seaborn**
* **Jupyter Notebook**



##  Conclusion

This project demonstrates how machine learning can be applied to historical datasets to gain insights and make predictions. It covers:

* End-to-end data preprocessing
* Feature engineering
* Model training and evaluation
* Real-world application through Kaggle


##  Author

**Maira Nawaz**

[LinkedIn](https://www.linkedin.com/in/mairanawaz/) | [Kaggle](https://www.kaggle.com/mairanawaz) | [Github](https://github.com/Maira-Nawaz)
