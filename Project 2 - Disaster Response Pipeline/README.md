# Disaster Response Pipeline 

## Introduction 
The goal of the project is to build a machine learning pipeline that is able classify the messages people send during the time of a natural disaster. In addition, an emergencey care works should have access to the classifcation ML model via a web frontend. Interacting with the frontend, a care work worker can input the message and get the message classified to one of the 36 categories 

## Folder and File Description 
* [ETL Pipeline Preparation.ipynb](https://github.com/TensorAdy/udacity_dsnd/blob/master/Project%202%20-%20Disaster%20Response%20Pipeline/ETL%20Pipeline%20Preparation.ipynb): Here experiments are run to build the piepline and push the trasnformed data into a datbase 
* [ML Pipeline Preparation.ipynb](https://github.com/TensorAdy/udacity_dsnd/blob/master/Project%202%20-%20Disaster%20Response%20Pipeline/ML%20Pipeline%20Preparation.ipynb): Here experiments are run to build a multiclass classifier and export the best model as a pickle file 
* process_data.py: This is script used for performing ETL on the data and storing the transformed data into a Sqllite database. This script is found in the *data* folder
* train_classifier.py: This is the script used to build, finetune, evaluate a model and to export it to pickle file that forms the basis for servinhg the model in production. This script is found in *model* folder  
* run.py: This is the script used for the web app, starting the server and prepare visualizations. This script is found in the *app* folder
* Data files : disaster_categories.csv, disaster_messages.csv, DisasterResponse.db all found the *data* folder
* App files : go.html, master.html found in the *app* folder inside templates folder 
* Model files : The actual pickle model could not be uploaded due to size constarints it's 100.3 mb but I have uploaded it to [Google Drive](https://drive.google.com/file/d/1YbsN7-XnlnaUClGkhrjCkUzM0WWQt_bx/view?usp=sharing)

## Reproducing the ML model and the app
1. ETL pipeline : `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
2. Model export  : `python model/train_classifier.py data/DisasterResponse.db models/classifier.pkl`
3. Web app : `python run.py` access the app via link shown after the script is run

### The UI endpoint 
![UI frontend of the app](https://github.com/TensorAdy/udacity_dsnd/blob/master/Project%202%20-%20Disaster%20Response%20Pipeline/app%20fontend%20-%20'I%20need%20water'.png)



