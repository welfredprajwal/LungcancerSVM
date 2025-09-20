🫁 Lung Cancer Detection using SVM


📌 Overview

This project uses Support Vector Machine (SVM), a supervised machine learning algorithm, to predict the likelihood of lung cancer based on demographic, lifestyle, and symptom data. Early detection of lung cancer is critical for effective treatment and improving patient outcomes.

The model uses features such as age, gender, smoking habits, chronic disease, fatigue, and other symptoms to classify patients as having lung cancer or not.

📂 Dataset

The dataset contains the following columns:

GENDER (Male/Female)

AGE	(Age of the patient in years)

SMOKING	Smoker (Yes=1 / No=0)

YELLOW_FINGERS	Presence of yellow fingers (Yes/No)

ANXIETY	Anxiety condition (Yes/No)

PEER_PRESSURE	Peer influence (Yes/No)

CHRONIC DISEASE	Presence of chronic diseases

FATIGUE	Fatigue symptom (Yes/No)

ALLERGY	Allergy history (Yes/No)

WHEEZING	Wheezing symptom (Yes/No)

ALCOHOL CONSUMING	Alcohol consumption (Yes/No)

COUGHING	Frequent coughing symptom

SHORTNESS OF BREATH	Breathlessness symptom (Yes/No)

SWALLOWING DIFFICULTY	Difficulty swallowing (Yes/No)

CHEST PAIN	Chest pain presence (Yes/No)

LUNG_CANCER	Target variable: 1 = Lung Cancer, 0 = No Lung Cancer


⚙️ Workflow

1.Data Preprocessing

  Encode categorical features (e.g., Gender: Male=1, Female=0).

  Scale features using StandardScaler (important for SVM).

2.Train-Test Split

  Split dataset into training (80%) and testing (20%) sets.

3.Model Training

  Train an SVM classifier using GridSearchCV for hyperparameter tuning (C, gamma, kernel).

4.Evaluation

  Accuracy, Precision, Recall, F1-score

  Confusion Matrix visualization


Expected Results

Accuracy: ~90–95% depending on dataset quality and preprocessing.

High recall for positive cases (lung cancer detection) is critical to avoid false negatives.
