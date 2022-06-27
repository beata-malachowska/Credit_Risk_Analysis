# Credit_Risk_Analysis

###Overview of the analysis

The purpose of this analysis was to credit risk based on client data using six supervised machine learning models.

###Results


![Random Over Samples - Logistic Regression](https://github.com/beata-malachowska/Credit_Risk_Analysis/blob/main/Classification_report_RandomOverSampler_LogisticRegression.png)

                   pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.66      0.66      0.80      0.66      0.44     17104
          1       0.01      0.66      0.66      0.02      0.66      0.44       101

avg / total       0.99      0.66      0.66      0.79      0.66      0.44     17205



![Cluster Centroids - Logistic Regression](https://github.com/beata-malachowska/Credit_Risk_Analysis/blob/main/Classification_report_ClusterCentroids_LogisticRegression.png)

                   pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.40      0.67      0.57      0.52      0.26     17104
          1       0.01      0.67      0.40      0.01      0.52      0.27       101

avg / total       0.99      0.40      0.67      0.56      0.52      0.26     17205


![SMOTE - Logistic Regression](https://github.com/beata-malachowska/Credit_Risk_Analysis/blob/main/Classification_report_SMOTE_LogisticRegression.png)

                   pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.68      0.61      0.81      0.65      0.42     17104
          1       0.01      0.61      0.68      0.02      0.65      0.42       101

avg / total       0.99      0.68      0.61      0.81      0.65      0.42     17205


![SMOTEENN - Logistic Regression](https://github.com/beata-malachowska/Credit_Risk_Analysis/blob/main/Classification_report_SMOTEENN_LogisticRegression.png)

                   pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.56      0.72      0.72      0.64      0.40     17104
          1       0.01      0.72      0.56      0.02      0.64      0.41       101

avg / total       0.99      0.56      0.72      0.71      0.64      0.40     17205



![BalancedRandomForest](https://github.com/beata-malachowska/Credit_Risk_Analysis/blob/main/Classification_report_BalancedRandomForest.png)

                   pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.84      0.56      0.91      0.69      0.49     17104
          1       0.02      0.56      0.84      0.04      0.69      0.46       101

avg / total       0.99      0.84      0.57      0.91      0.69      0.49     17205


![EasyEnsemble AdaBoost](https://github.com/beata-malachowska/Credit_Risk_Analysis/blob/main/Classification_report_EasyEnsemble.png)

                   pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.76      0.71      0.87      0.74      0.55     17104
          1       0.02      0.71      0.76      0.03      0.74      0.54       101

avg / total       0.99      0.76      0.71      0.86      0.74      0.55     17205

The balanced accuracy scores and the precision and recall scores were as following: 
- 0.66 0.01 0.66 (RandomOverSampler, Logistic Regression)
- 0.65 0.01 0.67 (Cluster Centroid, Logistic Regression)
- 0.53 0.01 0.61 (SMOTE, Logistic Regression)
- 0.64 0.01 0.72 (SMOTEEN, Logistic Regression)
- 0.70 0.02 0.56 (Balanced Random Forest)
- 0.74 0.02 0.71 (AdaBoost)


###Summary

Overall alll models prefromed poorly. Hghest precision reached 0.02 what is a very low value, meaning that there will be mane false positive results, Even though the precision for the best model reached 0.71 and the accuracy 0.74 (Ada Boost model) it is still to low to recommend using this model in daily practice. 
