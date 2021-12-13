# Heart-Disease-Classification
This project will demonstrate some foundation of machine learning and data science by exploring the problem of heart disease classification.
For our journey to learn data science, we were trilled to learn different techniques. Classification involves deciding whether a sample is part of one class or another (single-class classification). If there are multiple class options, it's referred to as multi-class classification.

We will approach the problem with the following machine learning modelling framework
![image](https://user-images.githubusercontent.com/16805149/145738339-d8aabd32-1e30-454a-b46a-1d2512b3f689.png)

6 Step Machine Learning Modelling Framework More specifically, we'll look at the following topics.

More specifically, we'll look at the following topics.
Exploratory data analysis (EDA) - the process of going through a dataset and finding out more about it.

> Model training - create model(s) to learn to predict a target variable based on other variables.
> Model evaluation - evaluating a models predictions using problem-specific evaluation metrics.
> Model comparison - comparing several different models to find the best one.
> Model fine-tuning - once we've found a good model, how can we improve it?
> Feature importance - since we're predicting the presence of heart disease, are there some things which are more important for prediction?
> Cross-validation - if we do build a good model, can we be sure it will work on unseen data? 7 Reporting what we've found - if we had to present our work, what would we show someone?


# 1. Problem Definition
We will be exploring binary classification which means a sample can only be one of two things. We are going use numbers of feautures about a person to predict whether they have heart disease or not.

Given clinical parameters about a patient, can we predict whether or not they have heart disease?

# 2. Data
The data is from Cleveland Database from UCI Machine Learning Repository The original database contains 76 attributes , here only 14 will be used for our project. Attributes (also called features) are the variables what we'll use to predict our target variable.

Attributes and features are also referred to as independent variables and a target variable can be referred to as a dependent variable.

We use the independent variables to predict our dependent variable.

Or in our case, the independent variables are a patients different medical attributes and the dependent variable is whether or not they have heart disease.

# 3. Evaluation
We want to reach 95% for accuracy at predicting whether or not a patient has heart disease during the proof of concept. if it is successful, we'll pursure this project.

# 4. Features
Features are different parts of the data. During this step, you'll want to start finding out what you can about the data.

One of the most common ways to do this, is to create a data dictionary.

Heart Disease Data Dictionary A data dictionary describes the data you're dealing with. Not all datasets come with them so this is where you may have to do your research or ask a subject matter expert (someone who knows about the data) for more.

The following are the features we'll use to predict our target variable (heart disease or no heart disease).

age - age in years
sex - (1 = male; 0 = female)
cp - chest pain type
 0: Typical angina: chest pain related decrease blood supply to the heart
 1: Atypical angina: chest pain not related to heart
 2: Non-anginal pain: typically esophageal spasms (non heart related)
 3: Asymptomatic: chest pain not showing signs of disease
trestbps - resting blood pressure (in mm Hg on admission to the hospital)
 anything above 130-140 is typically cause for concern
 chol - serum cholestoral in mg/dl
 serum = LDL + HDL + .2 * triglycerides
 above 200 is cause for concern
fbs - (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
 '>126' mg/dL signals diabetes
restecg - resting electrocardiographic results
 0: Nothing to note
 1: ST-T Wave abnormality
     can range from mild symptoms to severe problems
     signals non-normal heart beat
 2: Possible or definite left ventricular hypertrophy
     Enlarged heart's main pumping chamber
thalach - maximum heart rate achieved
exang - exercise induced angina (1 = yes; 0 = no)
oldpeak - ST depression induced by exercise relative to rest looks at stress of heart during excercise
unhealthy heart will stress more
slope - the slope of the peak exercise ST segment
0: Upsloping: better heart rate with excercise (uncommon)
1: Flatsloping: minimal change (typical healthy heart)
2: Downslopins: signs of unhealthy heart
ca - number of major vessels (0-3) colored by flourosopy
colored vessel means the doctor can see the blood passing through
the more blood movement the better (no clots)
thal - thalium stress result
1,3: normal
6: fixed defect: used to be defect but ok now
7: reversable defect: no proper blood movement when excercising
target - have disease or not (1=yes, 0=no) (= the predicted attribute)
Note: No personal identifiable information (PPI) can be found in the dataset.

It's a good idea to save these to a Python dictionary or in an external file, so we can look at them later without coming back here.

# Preparing the tools
we will use pandas Numpy Matplotlib and Scikit_Learn:

* pandas for data analysis.
* NumPy for numerical operations.
* Matplotlib/seaborn for plotting or data visualization.
* Scikit-Learn for machine learning modelling and evaluation.





