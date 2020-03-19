# Disaster Response Pipeline 

## Introduction 
The goal of the project is to build a machine learning pipeline that is able classify the messages people send during the time of a natural disaster. In addition, an emergencey care works should have access to the classifcation ML model via a web frontend. Interacting with the frontend, a care work worker can input the message and get the message classified to one of the 36 categories 

## Folder and File Description 
* ETL Pipeline Preparation.ipynb: Here experiments are run to build th epiepline and push the trasnformed data to a data base 
* ML Pipeline Preparation.ipynb: Here experiments are run to build a multiclass calassifier and export the best model as a pickle file 
* process_data.py: This is script user for performing ETL on the data and storing the trasnformed data into a Sqllite database. This script is found in the *data* folder  

