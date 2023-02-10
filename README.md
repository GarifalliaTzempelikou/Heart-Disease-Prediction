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
- We examine the feature selection ( Feature Importances, Shap, plot partial dependence, Select K Best (chi2), MRMR)
- We train some models and compare the metrics
- We improve our models with hyperparameter tuning to optimize the performance

## Let's have a taste 

Here are some insights of the feature selection process 

<img width="971" alt="Screenshot 2023-02-10 at 10 34 55 PM" src="https://user-images.githubusercontent.com/125039071/218192702-4d266ea5-c1e1-473e-9769-85f2d525c9b2.png">

These are top 10 features according to feature importances for Random Forest Classifier. 
It seems like the most important feature is BMI with AgeCategory and SleepTime following. Physical health and Mental health are also in the top 5 features which are important for heart disease. 


###### Now let's see our models perfomance.

<img width="893" alt="Screenshot 2023-02-10 at 11 04 37 PM" src="https://user-images.githubusercontent.com/125039071/218197281-73d49a33-293e-48d4-9ed0-f324fac77ef8.png">

The results above came from default-parameter performances. What is happening when we use hyperparameter tuning?


#### If you are intrested to see more about feature selection and the predictive-model choice check this project!

