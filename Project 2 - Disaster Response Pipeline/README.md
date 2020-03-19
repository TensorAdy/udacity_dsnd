# Disaster Response Pipeline 

## Introduction 
The goal of the project is to build a machine learning pipeline that is able classify the messages people send during the time of a natural disaster. In addition, an emergencey care works should have access to the classifcation ML model via a web frontend. Interacting with the frontend, a care work worker can input the message and get the message classified to one of the 36 categories 

## Folder and File Description 
* ETL Pipeline Preparation.ipynb: Here experiments are run to build the piepline and push the trasnformed data into a datbase 
* ML Pipeline Preparation.ipynb: Here experiments are run to build a multiclass calassifier and export the best model as a pickle file 
* process_data.py: This is script used for performing ETL on the data and storing the transformed data into a Sqllite database. This script is found in the *data* folder
* train_classifier.py: This is the script used to build, finetune, evaluate a model and to export it to pickle file that forms the basis for servinhg the model in production. This script is found in *model* folder  
* run.py: This is the script used for the web app, starting the server and prepare visualizations. This script is found in the *app* folder
* Data files : disaster_categories.csv, disaster_messages.csv, DisasterResponse.db all found the *data* folder
* App files : go.html, master.html found in the *app* folder


