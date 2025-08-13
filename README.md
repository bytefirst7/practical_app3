**Problem Statement / Business Objective:**

Evaluate and compare the performance of four classification models: K-Nearest Neighbors,
Logistic Regression, Decision Trees, and Support Vector Machines using a bank marketing
dataset to predict whether a client will subscribe to a term deposit.

**Understanding the Data:**
The data is based on more than one contact with the same client,
in order to access if the product (bank term deposit) would be
('yes') or not ('no') subscribed.

**Interpretation:**

**Baseline** - This model predicts the most frequent class. It simply serves as a reference point.

                      Model  Train Time  Train Accuracy  Test Accuracy
0  Baseline (Most Frequent)      0.0027          0.8876         0.8865

                      Model  Train Time  Train Accuracy  Test Accuracy
1       Logistic Regression      0.8760          0.9117         0.9115
0  Baseline (Most Frequent)      0.0027          0.8876         0.8865

**Simple Models**
Logistic Regression has high accuracy, and performance during training/testing is very fast. SVM has high train accuracy,
but test accuracy is slow.
KNN and Decision Tree perform very poorly.
Next Steps: Adjust SVM and Decision Trees models to account for overfitting.
 
                      Model  Train Time  Train Accuracy  Test Accuracy
1       Logistic Regression      0.8760          0.9117         0.9115
4                       SVM     33.9950          0.9282         0.9090
2                       KNN      0.0731          0.9199         0.8978
3             Decision Tree      0.3090          1.0000         0.8871

**Improved Models**
Logistic Regression continues to remain consistent and strong across multiple
metrics. Decision Tree models improves slightly by having a balance of
accuracy and F1 score. KNN is not suggested for this task at all
                 Model  Train Time  Test Accuracy  F1 Score  ROC AUC
2        Decision Tree     23.1369         0.9150    0.5916   0.9210
0  Logistic Regression      5.8870         0.9115    0.5245   0.9349
1                  KNN     40.7475         0.8966    0.3790   0.8199

                 Model  Train Time  Test Accuracy  F1 Score  ROC AUC
0        Decision Tree     25.5203         0.9150    0.5916   0.9210
1  Logistic Regression    127.6077         0.9111    0.5222   0.9350
2                  KNN     40.9229         0.8966    0.3790   0.8199

**Next steps:** Adjust models to account for overfitting, remove KNN totally because it is not ideal for this task.
