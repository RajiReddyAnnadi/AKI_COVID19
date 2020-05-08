# AKI_COVID19
Three main folders right now which are important.

1./AKI_hospital_prediction/
contains:
    AKI_COVID_data_AKI_pred.csv : contains "AKI during hospitalization? (y/n)" as target label which is specfied as 'Y'.
    aki_prediction.ipynb : parses and trains the XGBoost classifier.

2./Mechanical_Ventilation_prediction/
contains:
    AKI_COVID_data_mech_ventilation.csv : contains "Mechanical ventilation (y/n)" as target label which is specfied as 'Y'.
    mech_ventilation_prediction.ipynb : parses and trains the XGBoost classifier.

3./RRT_prediction/
contains:
    AKI_COVID_data_RRT_prediction.csv : contains "RRT (y/n)" as target label which is specfied as 'Y'.
    rrt_prediction.ipynb : parses and trains the XGBoost classifier.

The csv files in the above folders contain the feature type identifier row just after headers. They specify the type of the data of each feature. The different types of identifiers include:
    0 indicates categorical data.
    1 indicates numerical data.
    -1 indicates the feature needs to be preprocessed and converted into the above specfied type of data. (Eg: feature 'SBP/DBP on admission')
    Y indicates the particular feature is the target label.

Note: All the .ipynb files are having the same code except the file name of csv.