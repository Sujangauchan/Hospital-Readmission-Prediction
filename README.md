# Hospital-Readmission-Prediction

Main application: https://github.com/Sujangauchan/hospital-readmission-app

Initial Preprocessing and Merging: https://github.com/Sujangauchan/MIMIC-IV-Preprocessing-and-merging-for-Readmission-Prediction/tree/main

BERT based readmission text classifier finetuning process (Only the converged version- stopped by early stopping, loaded model checkpoint from 2 previous 12 hour runs): https://www.kaggle.com/code/surajgauchan/bert-finetuning-main/notebook 

Model Training for Tabular Data: https://www.kaggle.com/code/sujangauchan/train-and-test-model-structured/notebook?scriptVersionId=268103386

BERT based readmission text classifier finetuning process: https://www.kaggle.com/code/sujangauchan/stacking-classifier-hospital-readmission-mimic-iv

Model predictions on Validation set to get outputs to train the meta learner:  

    BERT:https://www.kaggle.com/code/sujangauchan/bert-admission-wise-prediction?scriptVersionId=267153909
    XGBOOST:https://www.kaggle.com/code/sujangauchan/xgboost-prediction-outputs-to-train-meta-learner?scriptVersionId=267365548

META Learner model training: https://www.kaggle.com/code/sujangauchan/meta-learner-logistic-regression-training?scriptVersionId=268062115

Final Stacking Model prediction and evaluation: https://www.kaggle.com/code/sujangauchansipradi/mimic-iv-stacking-hosp-readm?scriptVersionId=268331913
