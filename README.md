# DataClearnning-XGBoost-PregnancyMentalHealthCOVID19
Data Clearnning and XGBoost training on PregnancyMentalHealthCOVID19<br>
Below is the overview of the whole process.<br>
You can find the detailed process in [Stage1_DataCleaningReport](https://github.com/GarryGeng/DataClearnning-XGBoost-PregnancyMentalHealthCOVID19/blob/main/Stage1_DataCleaningReport.pdf) and [Stage2_XGBoostModelReport](https://github.com/GarryGeng/DataClearnning-XGBoost-PregnancyMentalHealthCOVID19/blob/main/Stage2_XGBoostModelReport.pdf).
## Data Clearning

1. **Normalization and Encoding**<br>
- One-hot encoding: Using in Language variable to retain informational value without binary reduction.<br>
- String-dated attributes were transformed into datetime objects to facilitate temporal analyses.<br>

2. **Fill the Missing Value By uisng**<br>
- Iterative Imputer with Random Forest Regressor, <br>
- K-nearest neighbors (kNN) algorithm, <br>
- Kernel Density Estimation (KDE)<br>

## Model Training

1. **Chooe Training Feature**<br>
- Set Edinburgh Postnatal Depression Scale (EPDS) and  PROMIS Anxiety as the predict feature. <br>

2. **Set Up XGBoost Model**<br>

3. **Fine Tune**<br>
- Using 'GridSearchCV' to fine tun the XGBoost Model.<br>

4. **Model Evaluation**
- F1 score
- Precision
- AUC-ROC
