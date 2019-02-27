# Fraud Detection using scikit-sklearn

The project mainly involved classification of unknown samples that were provided into two binary classes based on the conclusions that were derived from the training data. The dataset provided was highly imbalanced with 95% of the rows belonging to the negative class. 
Thus, various sampling strategies and stratification was employed to account for that. Because the data was highly imbalanced, model accuracy did not prove to be an appropriate metric for evaluating the models and thus, f-score and confusion matrix was used to judge the results obtained. 
The dataset had almost all the features being categorical and thus, quite a lot of preprocessing had to be done to make the data consumable by the models being used.
Various algorithms were tried and AdaBoost gave the best results as far as the confusion matrix was concerned.

`Dataset.csv` contains the data used for suprevised training which was further split into training and validation sets using K-Fold cross-validation and Startified K-fold cross validation. 

`Test.csv` contains data for which the target class, that is, FraudFound_P needs to be predicted.

`yPred.csv` are the results obtained for the `Test.csv` file using the AdaBoost Algorithm.

`EXL EQ.ipynb` conatins the python code for the various preprocessing methodologies employed and the corresponding experimentation with models to arrive at the final result.

