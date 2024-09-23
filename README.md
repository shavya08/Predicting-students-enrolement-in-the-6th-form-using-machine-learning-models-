# Predicting-students-enrolement-in-the-6th-form-using-machine-learning-models-

# Project Overview
This project aims to predict student enrollment in 6th Form (senior secondary education) by leveraging machine learning models to classify students into three categories:

Likely to Enroll
Unlikely to Enroll
Undecided

By analyzing various student attributes such as academic performance, socio-economic background, subject preferences, and geographic proximity, the models provide actionable insights to help schools optimize their recruitment strategies and resource allocation.

# Objectives
Develop predictive models to accurately classify students into three categories of enrollment likelihood.
Use historical data to improve decision-making for schools regarding recruitment and resource planning.
Provide insights to target interventions for students "on the fence" about enrolling.

# Methodology
The project utilizes several machine learning models:

Logistic Regression (chosen as the final model)
Random Forest
Decision Trees
XGBoost
Support Vector Machine (SVM)

Data Preprocessing
Managed missing values and class imbalance issues.
Categorical variables (such as subject preferences) were encoded.
Applied normalization to numeric features like geographic proximity to ensure model performance.

Model Training & Tuning
Applied hyperparameter tuning to optimize model performance.
Addressed class imbalance using techniques like SMOTE (Synthetic Minority Over-sampling Technique).
Split the data into training and test sets to validate the models effectively.

Model Evaluation Metrics
Accuracy: To measure the overall correctness of the model predictions.
Precision: To measure how many predicted enrollments were actually correct.
Recall: To measure how well the model identified all actual enrollments.
F1-Score: To provide a balance between precision and recall.

# Results
The models were evaluated based on their accuracy, precision, recall, and F1-score. Logistic Regression was chosen as the final model due to its strong balance across these metrics.

Logistic Regression achieved an accuracy of 82%, with a precision of 80% and recall of 78% for the "likely to enroll" category. Its F1-Score was 79%, making it a reliable choice for predicting student enrollment outcomes.

Random Forest performed slightly better on the "likely to enroll" category, with a 85% accuracy, but exhibited a slight drop in precision and recall for the "undecided" category, making it less balanced overall.

XGBoost demonstrated strong performance with a 83% accuracy and was particularly effective at handling the "undecided" category, achieving a precision of 82% but had slightly lower recall at 76%.

Decision Trees and SVM had lower overall performance, with accuracy metrics ranging between 75-78%, largely due to their sensitivity to class imbalance, despite efforts to mitigate this with techniques like SMOTE.

# Key Findings:
Academic performance and geographic proximity were the top predictive features, significantly influencing the likelihood of enrollment.
The undecided category was the most challenging to classify accurately, with models having lower recall for this group. Logistic Regression, however, managed to classify 76% of the undecided students correctly.
By optimizing hyperparameters and addressing class imbalances, the final Logistic Regression model provided a highly interpretable solution for school administrators.

# Technologies Used
Python for data preprocessing, model building, and evaluation.
Libraries used: pandas, numpy, scikit-learn, XGBoost
Excel for managing input/output datasets and initial data exploration.
Jupyter Notebooks for interactive model development and analysis.

# Visualizations
Confusion Matrices were generated to visualize model performance across all categories.
ROC Curves for evaluating the trade-off between true positive rates and false positive rates.
Bar Charts to illustrate the importance of various features in predicting enrollment.

# Key Takeaways
The final Logistic Regression model can accurately classify students likely to enroll, with a balanced trade-off between precision and recall.
Socio-economic background and proximity to the institution were among the top predictive factors influencing a student's decision to enroll.
The project’s models provide educational institutions with actionable insights to enhance targeted recruitment efforts.

# How to Use
Clone the Repository:
bash
Copy code
git clone https://github.com/your-repo/predicting-student-enrollment.git
Run the Models: The Python scripts include data preprocessing, training, and evaluation of machine learning models.
Visualize Results: Use the provided code to generate key performance metrics and visualizations.
Adjust Data Inputs: You can modify the dataset to include different features or new student data to see how the model adjusts.

# Future Work
Extend the model to predict long-term student success beyond enrollment.
Integrate additional socio-demographic factors to improve prediction accuracy.
Explore deep learning models for further performance improvements.
