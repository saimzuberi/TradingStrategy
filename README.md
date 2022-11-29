# TradingStrategy

Use the starter code file to complete the steps that the instructions outline. The steps for this Challenge are divided into the following sections:

Establish a Baseline Performance

Tune the Baseline Trading Algorithm

Evaluate a New Machine Learning Classifier

Create an Evaluation Report

## Step 1: Tune the training algorithm by adjusting the size of the training dataset.
To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your README.md file.

Original Testing Report of the SVM Model 3 Months

               precision    recall  f1-score   support

    -1.0       0.43      0.04      0.07      1804
     1.0       0.56      0.96      0.71      2288

    accuracy                           0.55      4092
    macro avg  0.49     0.50        0.39        4092 
    weighted avg 0.50   0.55        0.43        4092

Answer the following question: What impact resulted from increasing or decreasing the training window?

Testing Report of the SVM Model 24 Months

              precision    recall  f1-score   support

    -1.0       0.80      0.00      0.01      1229
     1.0       0.56      1.00      0.72      1565

    accuracy                           0.56      2794
    macro avg       0.68    0.50    0.36         2794 
    weighted avg    0.67    0.56    0.41         2794

Step 2: Tune the trading algorithm by adjusting the SMA input features.
Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your README.md file.

Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?

Original Testing Report of the SVM Model 4 Short Window and 100 Long Window

               precision    recall  f1-score   support

    -1.0       0.43      0.04      0.07      1804
     1.0       0.56      0.96      0.71      2288

    accuracy                           0.55      4092
   macro avg       0.49      0.50      0.39      4092
weighted avg       0.50      0.55      0.43      4092
Testing Report of the SVM Model 30 Short Window and 200 Long Window and 3 months training data

              precision    recall  f1-score   support

    -1.0       0.43      0.04      0.07      1804
     1.0       0.56      0.96      0.71      2288

    accuracy                           0.55      4092
   macro avg       0.49      0.50      0.39      4092
weighted avg       0.50      0.55      0.43      4092
Step 3: Choose the set of parameters that best improved the trading algorithm returns.
Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your README.md file.

Final Set of Parameters

SMA Short 30 SMA Long 200 Training Window 24 months

Original precision recall f1-score support

    -1.0       0.43      0.04      0.07      1804
     1.0       0.56      0.96      0.71      2288

    accuracy                           0.55      4092
   macro avg       0.49      0.50      0.39      4092
weighted avg       0.50      0.55      0.43      4092
Improved

                precision    recall  f1-score   support

    -1.0       0.46      0.42      0.44      1151
     1.0       0.57      0.61      0.59      1452

   accuracy                           0.53      2603
   macro avg       0.52      0.52      0.52      2603
weighted avg       0.52      0.53      0.53      2603