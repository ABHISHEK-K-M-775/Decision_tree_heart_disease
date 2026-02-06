Project title : Decsison tree heart desease

>In this project we will train a decision tree ML model to predict if a person has heaert disease using some features

EDA:

>To do the analysis we have taken heart.csv dataset  from kagle

>it is a small dataset of 302 samples and 14 features along with target features

>we named the features and done visual inspection on data such as shape, datatypes, describen isnull

>we found no missing data but 2 columns had datatypes as object beacuse of missing values with filled as '?'

>since the samples containing missing values are less compared to total size of dataset we simply drop those columns 

>we also note that there are no outliers in numerical columns

Feauture engineering 
>the dataset has no column name so we assign column names using domain knowledge
>we split tha data along axis=1 as dependent and independent features
>we had few columns whose data are nominal so we done one hot encoding on those columns
>and in target column had severity of heart disease from 0-4 so we simply modified them into had heart disease or not had heart disease 
 

Model training
>in model training we split both dependent and independent data into testing and traing

>and then we train our decsion tree classifier with xtrain and y train

>after model is trained we got the tree plot 
 
>from tree plot we see to many leaves and each leaf is pure, and most leaves have 1-2 samples so on surface it suggests that model is overfitted 
 
>classification report of the model:
             precision    recall  f1-score   support

           0       0.80      0.68      0.74        41
           1       0.67      0.79      0.72        33

    accuracy                           0.73        74
   macro avg       0.73      0.74      0.73        74
weighted avg       0.74      0.73      0.73        74

>

