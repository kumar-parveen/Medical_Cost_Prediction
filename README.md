# Medical_Cost_Prediction
This repository contains a machine learning project aimed at predicting medical expenses using patient information. Leveraging the Insurance dataset from Kaggle, the project develops decision tree, random forest, and linear regression models to forecast medical costs based on attributes such as age, gender, BMI, smoking status, etc.

My examination of healthcare expenditures utilizing the Medical Cost Personal Dataset provides a valuable perspective on the determinants impacting healthcare expenses in the United States. 
The dataset contains 1338 observations and 7 variables.

## Objective
My objective is to analyze the correlation between features and construct a model capable of forecasting medical costs. This endeavour aims to provide proactive insights to the healthcare system, aiding in the formulation of policies and strategies.

## Data Exploration 

### Rows & Columns

![shape](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/e80cf2af-eedc-4bef-a8a4-d01df3ae4d1b)

### Data Information

![datatypes](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/78c03a2b-e138-47aa-a6e4-59841bf7ba71)

I have discovered that the variables "sex, " "smoker, " and "region" are categorical in nature. Consequently, I will proceed to convert them into numerical format.

### Categorical to Numerical conversion

![categoricaltonumerical](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/7e608314-799b-493a-bfc8-c2d1d1cdc3ab)

### 5 Point Summary

![coorelation](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/5f796d24-e056-41b3-992e-257e350eb1f0)

### Gender Distribution (Almost Equal)

![Gender Distribution](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/bcc1127f-f14e-4194-add7-56dad8b9dfd3) 

### BMI distribution (Between 25 to 40, overweight)

![BMI Distribution](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/4e0ccd7d-72b5-4355-8472-969916b0d165)




## Exploratory Data Analyusis 

### Age distribution (Max 19 year age)

![Age Distribution](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/6d5c89f6-8f89-4a69-821c-b889a1021f75)

### Smoker Distribution (Almost 80% are non smokers)

![Smoker Count](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/0a787405-5d77-4605-9a74-53c1a8a5c48c)

### Charges distribution (Most of the expenses below 20000)

![Charges Distribution](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/d7f99861-0175-480e-a76c-31dacf63819b) 

### Region Distribution,SE have slightly higher no. of patients

![Region Distribution](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/78ef0352-cce4-4b09-881a-a0916d759f17)

## CORRELATION
### Correlation heat map,The variable smoker shows a significant correlation with medical expenses

![coorelationheatmap](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/71ee52c3-e856-4486-b2c5-9ebc661f9f82)

## DATA VISUALISATION

### GENDER SMOKER COUNT

The gender smoker count Clearly describes more male smokers than female smokers. So I will ensure that more expenses will be for male patients than females.

![Smoker count with gender](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/26cd2003-c881-4a4c-b035-70ca0a4b1319)

### BOX PLOT FOR FEMALE EXPENSES

![womencharges](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/6d36e974-91ff-48f8-871f-8b14387111df)

### BOX PLOT FOR MALE EXPENSES 

![malecharges](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/93a7131c-7c9c-4f15-abae-f983906316b0)

### SMOKER AND AGE DISTRIBUTION

![smokeragedistribution](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/1764dda6-5285-40d9-aa8d-6cdb42645565)

From the graph, We can see that there significant number of smoker of age 19.

### BOX PLOT FOR CHARGES OF SMOKERS OF AGE 19

![smokerage19](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/e316d81c-edfb-4375-b6d7-2bb56555a18c)

Surprisingly, The Medical expense of smokers of age 19 is very high in comparison to non smokers.

The Medical Expense of smokers is higher than that of non - smokers. 
Now let’s plot the charges distribution concerning patients ages of smokers and non – smokers.

## SCATTER PLOT FOR CHARGES OF NON SMOKERS

![scatterplotfor nonsmokercharges](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/c1f0a75c-f1d3-479f-92af-34da30037018) 

Majority of the points show that medical expense increases with age which may be due to the fact that older people are more prone to illness. 
But there are some outliners which shows that there are other illness or accidents which may increase the medical expense.

## SCATTER PLOT FOR CHARGES OF SMOKERS

![scatterplotforsmokercharges](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/d0d32cbd-fcd9-4c54-9332-7ff84aff8356)

In the graph, there are two segments, one with high medical expenses which may be due to smoking related illness and the other with low medical expenses which may be due age related illness.

## COMBINED GRAPH

![combinedsmokersnonsmokergraph](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/1dbb64f2-a8cc-4bc4-8724-6a20bbcf59ae)

Now let’s plot the charges distribution concerning patients ages of smokers and non – smokers.
Now, we clearly understand the variation in charges with respect to age and smoking habit. The
medical expense of smokers is higher than that of non - smokers. In non-smokers, the cost of
treatment increase with age which is obvious. But in smokers, the cost of treatment is high even
for younger patients, which means the smoking patients are spending upon their smoking related illness as well as age related illness.

## CHARGES DISTRIBUTION FOR PATIENTS
### WITH BMI > 30 I.E. OBESE PATIENTS

![chargesdistributionobesepeople](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/15a38f14-eaf7-46d3-b64e-026b83c7f140)


## CHARGES DISTRIBUTION FOR PATIENTS
### WITH BMI < 30 I.E. HEALTHY PATIENTS

![chargesdistributionnonobesepeople](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/96eb35f8-7d93-4fa3-90f1-8bf63dc18bc7)

Therefore, patients with BMI less than 30 are spending less on medical treatment than those with BMI greater than 30.


## MODEL BUILDING

### LINEAR REGRESSION

![linearregression](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/3f408a26-95ac-4fcd-8868-2efc8c92853c)

### POLYNOMIAL REGRESSION

![polynomialregression](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/df0b2d8a-80db-4884-95cc-24126a45f675)

### DECISION TREE REGRESSION

![decisiontreeregression](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/63fd9dcb-112a-4057-bfef-32493079afe2)

### RANDOM FOREST REGRESSOR

![randomforestregressor](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/e432337d-af5a-4de4-b97d-43e768a7cb61)

## RESULT

### LINEAR REGRESSION

![linearregr2score](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/91794a50-d710-4b24-944d-5f5042934074)

![actualvspredictedlinear](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/7ac08c8b-d22c-43e0-a7ac-1e6168c228b5)

### POLYNOMIAL REGRESSION

![r2scorepolynomial](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/7d819a1d-c0c4-417e-92b8-83b1bb4df43f)

![actualvspredictedpolynomial](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/d0659bce-a076-429d-91a1-c739eadfba44)

### DECISION TREE REGRESSION

![r2scoredecisiontree4](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/5cd98223-83fb-4b2c-a7a7-1adfe111723e)

![actualvspredicteddecisiontree](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/e7ae825c-90c4-4d5a-9e84-b403764bcdb7)


### RANDOM FOREST REGRESSOR

![r2scorerandomforest](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/7e950eec-ac83-4f24-8248-77dc3dd15279)

![actualvspredictedrandomforest](https://github.com/kumar-parveen/Medical_Cost_Prediction/assets/84096099/2910ed13-ffb1-4f1f-b6d5-cd9a4c019679)

## CONCLUSION

From the above models, we can see that Decision Tree Regressor and Random Forest Regressor are giving the best results. However, Random Forest Regressor gives the best results with the least RMSE value. 

Therefore, I will use a Random Forest Regressor to predict the medical expenses of patients. Moreover, the medical expense of smokers is higher than that of non-smokers. The medical expense of patients with a BMI greater than 30 is higher than that of patients with a BMI less than 30. 

The medical expenses of older patients are higher than that of younger patients. Thus, from the overall analysis, we can conclude that the medical expense of patients depends on their age, BMI, and smoking habits











