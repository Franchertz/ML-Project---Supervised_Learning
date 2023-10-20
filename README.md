# MACHINE_LEARNING_PROJECT - SUPERVISED-LEARNING


### PROBLEM STATEMENT

The objective of this project is to develop a predictive model for diagnosing
diabetes in female patients of Pima Indian heritage, aged at least 21 years.
The model's task is to predict whether a patient has diabetes (Outcome = 1)
or does not have diabetes (Outcome = 0) based on several diagnostic measurements,
including glucose level, blood pressure, skin thickness, insulin level, BMI,
diabetes pedigree function, and age.

### PROJECT DESCRIPTION:

This project involves the application of supervised learning techniques to
real-world data, supported by data visualization tools to convey insights
gained from the analysis.

Diabetes is a group of metabolic disorders characterized by elevated blood sugar
levels over an extended period. Symptoms of high blood sugar include frequent
urination, increased thirst, and heightened hunger. If left untreated,
diabetes can lead to various complications, including acute ones like diabetic
ketoacidosis, hyperosmolar hyperglycemic state, and even death.
Long-term complications encompass cardiovascular disease, stroke,
chronic kidney disease, foot ulcers, and damage to the eyes.

The dataset used for this project, 'diabetes.csv', originates from the National
Institute of Diabetes and Digestive and Kidney Diseases. Its primary goal is to
predict diagnostically whether a patient has diabetes or not, based on specific
diagnostic measurements included in the dataset. Several constraints were applied
in the selection of instances from a larger database, including that all patients
are female, at least 21 years old, and of Pima Indian heritage.

The project's core objectives are as follows:


## PROJECT/GOALS

1. To employ supervised learning techniques in constructing a machine
   learning model capable of predicting whether a patient has diabetes
   based on diagnostic measurements.

2. To communicate the insights and model predictions effectively to
   stakeholders using appropriate visualization and evaluation metrics.


## PROCESS

### STEP 1: EXPLORATORY DATA ANALYSIS (EDA)

- 1. Upload dataset: `diabetes.csv`
    
    1. Dataset Upload: The dataset, 'diabetes.csv', is uploaded.
       It consists of various medical predictor variables and one
       target variable, Outcome, which denotes the presence (1) or
       absence (0) of diabetes.

    2. Data Cleaning.

    3. Data Visualization: Visualizing data patterns and correlations.

    4. Data Preparation for Modelling.

    5. Answering Questions.

### STEP 2: PREPROCESSING & FEATURE ENGINEERING 


    1. Handling Missing Values.

    2. Handling Outliers.

    3. Scaling and Normalization.

    4. Feature Engineering.

    5. Handling Imbalanced Data.


### STEP 3: TRAIN ML MODEL

    1. Model Training: Training selected models on the training dataset.

    2. Model Evaluation: Assessing the trained models on the testing dataset,
       utilizing appropriate evaluation metrics (e.g., accuracy, precision,
       recall, F1-score, ROC-AUC).

    3. Improving Model Performance: Additional analysis, including
       model tuning and cross-validation.

    4. Model Comparison: Comparing the performance of the selected
       models and selecting the best-performing model based on evaluation metrics.


### STEP 4: CONCLUSION

Exploratory Data Analysis (EDA) Insights:

- During our exploration of the data, the following were observed:

1. "BloodPressure" values typically lie between 40 and 100, and there
    are fewer diabetic cases in this range.

2. Pair plots reveal several insights, such as the relationship between
   pregnancy, high Glucose, and diabetes, and how increasing insulin
   and glucose levels are associated with higher chances of diabetes.

3. Age alone isn't a strong indicator of diabetes, as there's no clear
    linear relationship between age and diabetes.

4. Middle-aged individuals with high Glucose and BloodPressure levels
    have higher chances of diabetes, as seen in the scatter plot.

5. The average "Glucose" levels for non-diabetic and diabetic patients
    are around 109 and 141, respectively. Similarly, the average "BMI"
    for non-diabetic and diabetic patients is around 30 and 35, respectively.

Machine Model Insights:

1. The Random Forest model, after hyperparameter tuning,
   is the best choice for achieving high predictive accuracy.
2. It has improved performance, reduced overfitting,
   and outperforms the other models in both training and
   validation accuracy.
3. Logistic Regression performs reasonably well,
   with a balanced accuracy but slightly lower overall accuracy.
4. SVC exhibits high training accuracy but has overfitting
   issues and lower validation accuracy.

## RESULTS

Based on the analysis conducted in this project, the solution for the problem statement,
which aims to develop a predictive model for diagnosing diabetes in female patients
of Pima Indian heritage, aged at least 21 years, can be summarized as follows:

1. **Data Collection and Preprocessing:**
   - The project begins with the collection of a dataset containing
     diagnostic measurements for female patients.
   - The dataset is cleaned, and missing values are handled.
   - Outliers are addressed, and feature scaling and normalization
     are performed.
   - The data is prepared for modeling.

2. **Exploratory Data Analysis (EDA):**
   - Extensive EDA is conducted to gain insights into the data.
   - Important observations, such as the imbalance in the target
     variable, the presence of outliers in the "Insulin" feature,
     and right-skewed distributions of "Insulin" and "DiabetesPedigreeFunction,"
     are identified.
   - Correlations between features are analyzed, and the relationship
     between feature variables and the target variable is explored
     through visualizations.

3. **Model Building and Evaluation:**
   - Three machine learning models are selected for building
     predictive models: Support Vector Classifier (SVC), Logistic Regression,
     and Random Forest.
   - Each model is trained on the dataset, and training and validation
     accuracies are evaluated.
   - The models' performance is compared, and key findings include
     overfitting in SVC, a balanced but lower accuracy in Logistic Regression,
     and improved accuracy and reduced overfitting in Random Forest
     after hyperparameter tuning.

4. **Solution Recommendations:**
   - The analysis suggests that the Random Forest model, after
     hyperparameter tuning, provides the best solution for diagnosing
     diabetes in female patients.
   - It offers the highest training and validation accuracies,
     improved generalization, and a balanced performance.
   - Logistic Regression also provides reasonable results with
     balanced accuracy.
   - SVC exhibits overfitting and a lower validation accuracy.

The recommended solution is to deploy the Random Forest model for predicting
diabetes in female patients based on the provided diagnostic measurements.
Further deployment and testing in a real-world clinical setting are essential
to assess the model's effectiveness in practice. Additionally, continuous
monitoring and model updates may be necessary to improve and maintain predictive accuracy.

 