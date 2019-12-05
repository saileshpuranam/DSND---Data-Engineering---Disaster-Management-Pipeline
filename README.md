
# Disaster Response Pipeline

### Project Motivation and Objective

In this project, I have implemented ETL pipelines, NLP Pipelines and ML Pipelines to analyze disaster data from Figure Eight and build a model for an API that classifies disaster messages.

### Github Repo Contents

#### Data Folder
Raw datasets in csv format - disaster_categories & disaster_messages
process_data.py -  This program reads input data, performs ETL logics and generates the databasefile
DisasterResponse.db - Database created from transformed and cleaned data.

#### Models Folder
DisasterResponse.db - Database created from transformed and cleaned data.
train_classifier.py - This program loads data from above database, transforms it using NLP pipeline, Builds and trains ML pipeline which uses GridSearchCV 
classifier.pkl - Model output file in Pickle format

#### App Folder
classifier.pkl - Model output file in Pickle format
run.py: Flask app and the user interface used to predict results and display them.

#### ETL Pipeline Preparation
Jupyter Notebook with ETL pipeline preperation

#### ML Pipeline Preparation
Jupyter Notebook with NLP and ML pipeline preperation

#### Snaphots of Flask app outputs from browser
Three snapshots with Output Visualizations
One snapshot with message calssifying suggestions

#### README
Readme file with Github repo contents and detailed explanations

### Codes to run in CMD Terminal

cd /home/workspace/data

python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db

cd /home/workspace/models

python train_classifier.py ../data/DisasterResponse.db classifier.pkl

cd /home/workspace/app

python run.py

env|grep WORK

### Acknowledgements and Licensing

Datatsets for this project are exctracted through the Udacity course platform in collaboration with partners Figure Eight. 

Feel free use the codes, apps and other info in this repo for all your references whenever required.
