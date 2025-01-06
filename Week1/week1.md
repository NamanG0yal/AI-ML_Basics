First of all , an appropiate database containing variable names and non-biased data was found and used.
Normalisation and imputation is implemented.Imputation method seemed better than using the other methods to remove the empty values(though there wasn't any such missing value in the database).The used of feature engineering isn't beneficial as the data used can't be further broke down, insetead it might degrade our model, thus its not implemented.Encoding to categorial variables was also not required as it was already implemented.Then SMOTE was implemented as it seemed to be the best under the situation of our model to take care of class imbalance.Then Logical Regression, Random Forests, XGBoost and SVM algorithms are implemented.Each model was evaluated using the accuracy score and confusion matrices. The comparison showed that the Random Forest method suits the best to our model.As the class imbalance was already implemented, use of precision-recall score, according to me, is reduntant and observable in the confusion Matrices. Also, Lightgbm was not implemented as it would be quite time consuming, and that our data isn't skewed enough to make it necessary to use it, as we didn't implement further feature and model evaluations.
Results-
Accuracy scores-
RF-0.867
LR-0.62
SVM- 0.60
XGBoost-0.834
Confusion Matrices-
LR-
    0     1
0  2834  1856
1  1694  2962
RF- 
     0     1
0  4116   574
1   667  3989
SVM-
      0     1
0  3011  1679
1  2014  2642
XGB-
      0     1
0  4080   610
1   941  3715
**Thus Random Forest method seems the most appropiate
