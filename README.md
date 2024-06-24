# Data-Analytics

## Abstract or Overview. 
The main purpose of this project was to create a model that would predict a patient's length of hospital stay based on various admission factors, such as age, admission type, condition, etc. By determining an estimated length of stay, both hospital staff and the patient are able to prepare themselves for the estimated admission timeline.

## Stakeholder
From the patient perspective, knowing an approximate timeframe of how long you will be in the hospital is helpful. It can provide the ability to notify your work, make childcare arrangements, inform loved ones, budget for an estimated hospital bill, and more. For the healthcare providers, this enables them to know how many additional patients they can take on, arrange for the transition of care if necessary, and get a better idea of the length of stay for similar patients. It is also useful for hospital staff, who might need the information for capacity tracking or billing purposes.

## Data Description
This data was pulled from Kaggle. It is an artfical recreation of real patient data. As patient data is considered PHI, and therefore protected by HIPAA, only simulated data may be used. While this did create some challenges in terms of the model's accuracy, it required very little preprocessing/cleaning.

## Algorithm
This model works by taking user input for'Admission Type', 'Medical Condition', 'Gender', 'Doctor', 'Insurance Provider', 'Hospital', and 'Age' of the patient and using them to predict how long a patient's hospital stay will be. Using a RandomForestRegression model, it was able to predict the length of stay within an average of 8 days.

## Tools
For this project, I primarily used the following:
1. Pandas: used for dataframes and data analysis
2. Skit-Learn: for preprocessing, training, testing, cross-validation, and predictions
3. Pickle: saving and loading the files
4. Streamlit: creating the web app

## Ethical Concerns
The main ethical concern when it comes to this model is the potential of introducing unconcious bias. If a patient has a predicted length of stay that is higher than average, they may have their quality of care impacted unintentionally by the staff. Hospitals might not want to take on patients they know will consume a large amount of the organization's time and resources. The best method of prevention would be continued education of staff and caregivers on bias and proper patient care. As is the case with all protected health information, the most important factor in mitigating risks is ensuring that we are only accessing the information we need when we need it.
