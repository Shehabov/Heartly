# Heartly

## Overview
Heart attack is the second cause of disability in the world. CVD is rapidly increasing day by day, as stated by WHO. Cardiovascular-related problems cause 31% of worldwide deaths. Thus, it's increasingly necessary to be able to identify health habits and symptoms that contribute to heart attacks.

<center><img src='https://i.pinimg.com/originals/87/45/76/874576ebe081d0b3cc15c1a519dcb6c1.gif'></center>


## Problem Statement
In a statement,

> Given clinical parameters about a patient, can we understand the most correlated attributes and reasons for heart disease? can we also build an accessible and usable web app that allows users to key in their data and see if they have a risk of having a heart attack or not?


## Installation

```
Install pip requirements
```

```
pip install -r requirements.txt
```

```
python app.py
```

## Data
This dataset was created by combining different datasets already available independently but not combined before. In this dataset, 5 heart datasets are combined over 11 common features by IEEE scholars which makes it the largest heart disease dataset available so far for research purposes. The five datasets used for its curation are:

- Cleveland: 303 observations
- Hungarian: 294 observations
- Switzerland: 123 observations
- Long Beach VA: 200 observations
- Stalog (Heart) Data Set: 270 observations

The Dataset Can be accessed directly from IEEE Datasets. <br>
https://ieee-dataport.org/open-access/heart-disease-dataset-comprehensive#files

| Feature | Description |
| :- | :- |
| Age | age of the patient [years]
| Sex | sex of the patient [M: Male, F: Female]
| ChestPainType | chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
| RestingBP | resting blood pressure [mm Hg]
| Cholesterol | serum cholesterol [mm/dl]
| FastingBS | fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
| RestingECG | resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
| MaxHR | maximum heart rate achieved [Numeric value between 60 and 202]
| ExerciseAngina | exercise-induced angina [Y: Yes, N: No]
| Oldpeak | oldpeak = ST [Numeric value measured in depression]
| ST_Slope | the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
| HeartDisease | output class [1: heart disease, 0: Normal]

## Files

### Prototype
- `hearty.xd`: Contains the wireframe, the design system, and the prototype of 5 different device sizes.

### System Files
- Data analysis - EDA:
	- `cardiovascular disease.csv`: the dataset provided by IEEE and used for the project.
	- `EDA - Heartly.ipynb`: a notebook that contains advanced data analysis and visualization to uncover the underlying reasons for the heart attack based on the observations and the attributes of the dataset.
 
- Machine learning model:
	- `Machine Learning Model.ipynb`: a notebook that contains the classification model used for this project (KNN) along with the validation and evaluation of it.

- Web application:
	- pickleFiles: <br>
	              -- `cardiovascular disease.csv`: the dataset provided by IEEE and used for the project. 
	

- `Heart_Disease_Classification.ipynb`: contains the code of data exploration, preparation and modeling. 
- `model.pkl`: the classification model. 
- `heart_disease_app.py`: Flask API that bind between the classification model and the web page. 
- templates:
	- `Heart Disease Classifier.html`: a web page that contains a form for heart disease testing.
