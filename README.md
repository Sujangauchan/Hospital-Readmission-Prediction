# Hospital-Readmission-Prediction

## Introduction 

Multi-Modal Stacking Ensemble for Hospital Readmission Prediction: Integrating Clinical Notes and Tabular Data
Multi-Modal Stacking Ensemble for Hospital Readmission Prediction: Integrating Clinical Notes and Tabular Data
Developed an end-to-end ensemble predictive modeling pipeline focused on 30-day hospital readmissions by combining structured EHR data with unstructured clinical notes from the MIMIC-IV dataset, using a tailored setup of XGBoost for tabular features and a fine-tuned Bio_Discharge_Summary_BERT model for discharge summaries. 

The project involved building, testing, and refining these two models as independent components and then integrating them through a logistic regression meta-learner, allowing the system to merge probability outputs and produce a more balanced prediction. 

The full workflow covered data cleaning, feature preparation, model training, hyperparameter tuning, and performance evaluation across multiple benchmarks, resulting in the BERT classifier achieving the highest AUC score of 0.753 while the stacked model delivered the strongest precision-recall balance with highest F1-Score of 0.483. 

Additional SHAP-based interpretation highlighted previous admissions and abnormal lab events as key drivers of readmission risk. 

## Links

Main application: https://github.com/Sujangauchan/hospital-readmission-app

Initial Preprocessing and Merging: https://github.com/Sujangauchan/MIMIC-IV-Preprocessing-and-merging-for-Readmission-Prediction/tree/main

BERT based readmission text classifier finetuning: https://www.kaggle.com/code/surajgauchan/bert-finetuning-main/notebook (This is only the converged model loaded from previously finetuned model which has already undergone 24 hours of finetuning through 2 different 12 hour runs)

Model Training for Tabular Data: https://www.kaggle.com/code/sujangauchan/train-and-test-model-structured/notebook?scriptVersionId=268103386

BERT based readmission text classifier finetuning process: https://www.kaggle.com/code/sujangauchan/stacking-classifier-hospital-readmission-mimic-iv

Model predictions on Validation set to get outputs to train the meta learner:  

1. BERT:https://www.kaggle.com/code/sujangauchan/bert-admission-wise-prediction?scriptVersionId=267153909
2. XGBOOST:https://www.kaggle.com/code/sujangauchan/xgboost-prediction-outputs-to-train-meta-learner?scriptVersionId=267365548

META Learner model training: https://www.kaggle.com/code/sujangauchan/meta-learner-logistic-regression-training?scriptVersionId=268062115

Final Stacking Model prediction and evaluation: https://www.kaggle.com/code/sujangauchansipradi/mimic-iv-stacking-hosp-readm?scriptVersionId=268331913
