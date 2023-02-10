# Heart-Disease-Prediction
## Can we predict if a person has heart disease according to several features? 

![image](https://user-images.githubusercontent.com/125039071/218186648-10f14f22-72c3-4059-a0ab-d0e30f59b991.png)

In this project we trained a model using data of 400k adults related to their health status. The purpose of this research is to find the best performing model to make predictions.

# About Dataset

### What topic does the dataset cover?
(2020 annual CDC survey data of 400k adults related to their health status)

According to the CDC, heart disease is one of the leading causes of death for people of most races in the US (African Americans, American Indians and Alaska Natives, and white people). About half of all Americans (47%) have at least 1 of 3 key risk factors for heart disease: high blood pressure, high cholesterol, and smoking. Other key indicator include diabetic status, obesity (high BMI), not getting enough physical activity or drinking too much alcohol. Detecting and preventing the factors that have the greatest impact on heart disease is very important in healthcare. Computational developments, in turn, allow the application of machine learning methods to detect "patterns" from the data that can predict a patient's condition.

#### The columns

- HeartDisease : Respondents that have ever reported having coronary heart disease (CHD) or myocardial infarction (MI)
- BMI : Body Mass Index (BMI)
- Smoking : Have you smoked at least 100 cigarettes in your entire life? [Note: 5 packs = 100 cigarettes]
- AlcoholDrinking : Heavy drinkers (adult men having more than 14 drinks per week and adult women having more than 7 drinks per week)
- Stroke : (Ever told) (you had) a stroke?
- PhysicalHealth : Now thinking about your physical health, which includes physical illness and injury, for how many days during the past 30 was your physical health not good?
- MentalHealth : Thinking about your mental health, for how many days during the past 30 days was your mental health not good?
- DiffWalking : Do you have serious difficulty walking or climbing stairs?
- Sex : Are you male or female?
- AgeCategory : Fourteen-level age category

(source : kaggle)


# In this project

- We examine our dataset (null values, data types, outliers, correlation heatmap, target distrbution) 
- We clean our dataset (data type changes, get dummies)
- We examine the feature importances ( Feature Importances, Shap, plot partial dependence, Select K Best (chi2), MRMR)
- We train some models and compare the metrics
- We improve our models with hyperparameter tuning to optimize the performance

## Let's have a taste 

Here are some insights of the feature selection process 

<img width="971" alt="Screenshot 2023-02-10 at 10 34 55 PM" src="https://user-images.githubusercontent.com/125039071/218192702-4d266ea5-c1e1-473e-9769-85f2d525c9b2.png">

These are top 10 features according to feature importances for Random Forest Classifier. 
It seems like the most important feature is BMI with AgeCategory and SleepTime following. Physical health and Mental health are also in the top 5 features which are important for heart disease. 



<img width="1011" alt="Screenshot 2023-02-10 at 10 35 29 PM" src="https://user-images.githubusercontent.com/125039071/218192569-73ad3dcb-67da-4e24-be28-9c5385d36b50.png">

How do these features affect the target value (heart disease)? We clearly see that how old are you infuences to a great extent the occurrence of heart disease.

#### If you are intrested to see more about feature selection and the prediction model choice check this project!

