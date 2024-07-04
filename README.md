# Capstone-Project

Description
This project aims to develop predictive models that accurately forecast individuals at high risk of stroke using biometric data and other relevant factors. By leveraging these models, we aim to enhance preventive measures and reduce the incidence of strokes in the future.

Data Preprocessing
Our preprocessing steps included:

Handling Missing Values: Imputed missing BMI values with the median and smoking status with ratios matching the original dataset.
Encoding Categorical Variables: Converted categorical variables (gender, marital status, work type, residence type, smoking status) into dummy variables.
Normalizing Continuous Variables: Standardized age, average glucose level, and BMI.
Data Splitting: Divided the dataset into training and testing sets (80-20 split) for model evaluation.
Model Training
We trained three models with the following configurations:

DecisionTreeClassifier:
Hyperparameters: criterion='gini', max_depth=40, max_features='log2', min_samples_leaf=1, min_samples_split=5, random_state=42
RandomForestClassifier:
Hyperparameters: n_estimators=200, max_depth=20, min_samples_split=2, min_samples_leaf=1, random_state=42
KNeighborsClassifier:
Hyperparameters: n_neighbors=1


Evaluation
The models were evaluated using various performance metrics including accuracy, precision, recall, and f1-score. Confusion matrices were also plotted to visualize the performance.

Results
RandomForestClassifier: Achieved the best performance with an accuracy of 0.9967 on the test data.
Key Predictors: Age, average glucose level, and BMI were identified as the most significant predictors of stroke risk.


Future Work
Future improvements include:
Incorporating larger and more diverse datasets to improve model generalizability.
Exploring advanced modeling techniques such as ensemble learning and neural networks.
Integrating real-time data from wearable health devices for continuous monitoring and early intervention.
Collaborating with healthcare professionals to validate and fine-tune the models in clinical settings.

Conclusion
This project successfully developed and validated predictive models for stroke risk using machine learning techniques. The models, particularly the Random Forest, demonstrated high accuracy and reliability, highlighting their potential for practical application in clinical settings to aid in early identification and preventive care.