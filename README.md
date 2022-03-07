# Credit_Risk_Analysis

## Analysis Overview
In this project, we use Python to build and evaluate several machine learning models to predict credit risk.\
We adopted the following procedure:
- oversample the data using the **RandomOverSampler** and **SMOTE** algorithms.
- Undersample the data using the **ClusterCentroids** algorithm.
- Use a combinatorial approach of over- and undersampling using the **SMOTEENN** algorithm.
- Compare two machine learning models that reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**.

We will evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Resources
- Data Source: LoanStats_2019Q1.csv
- Software: Python 3.7.9, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results
### Naive Random Oversampling
![image](https://user-images.githubusercontent.com/92435456/156948824-4ffb3f94-b782-45ba-b5ad-9948a457a729.png)

The accuracy score is 62.9%.
The high risk precicion is about 1% with a sensitivity of 57%, which makes a F1 of only 2%. 
Due to the high volume of low risk population, the precision is almost 100% with a sensitivity of 68%.

### Smote Oversampling
![image](https://user-images.githubusercontent.com/92435456/156948832-96495db5-45bf-4d33-bacc-beaba2a6deb0.png)

The accuracy score is 62.7%.
The high risk precisions is about 1% with a sensitivity of 62%, which makes an F1 of only 2%. 
Due to the volume of low risk population, the precision is almost 100% with a sensitivity of 63%.
Similar results to the random sampling. 
### Undersampling
![image](https://user-images.githubusercontent.com/92435456/156948790-49b3dbfb-dd68-42d9-916a-3089e98b56d2.png)

The accuracy score is 59%.
The high risk precicion is about 1% with a sensitivity of 61%, which makes a F1 of only 1%. 
Due to thevolume of low risk population, the precision is almost 100% with a sensitivity of 57%.
### Combination Sampling
![image](https://user-images.githubusercontent.com/92435456/156948812-9dac4e61-96dc-4123-be84-eb832d65369c.png)

The accuracy score is 65.4%.
The high risk precicion is about 1% with a sensitivity of 70%, which makes a F1 of only 2%. 
Due to the high volume of low risk population, the precision is almost 100% with a sensitivity of 61%.
