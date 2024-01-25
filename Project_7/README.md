Disaster Response Pipeline Project

Project Description
In this project, I will create a machine learning/NLP pipeline to categorize these events and build a model to classify messages that are sent during disasters. There are 36 pre-defined categories, and examples of these categories include Aid Related, Medical Help, Search And Rescue, etc. By classifying these messages, we can allow these messages to be sent to the appropriate disaster relief agency. The dataset -provided by Figure Eight- is used to build a model that classifies disaster messages, while the web app is where a respondent can input a new message and get classification results in several categories.

Finally, this project also contains a web app that allows you to input a message and get classification results.

File Description



       

      {disaster_response_pipeline
          |-- app
                |-- templates
                        |-- go.html
                        |-- master.html
                |-- run.py
          |-- data
                |-- disaster_message.csv
                |-- disaster_categories.csv
                |-- DisasterResponse.db
                |-- process_data.py
          |-- models
                |-- classifier.pkl
                |-- train_classifier.py
          |-- Preparation
                |-- categories.csv
                |-- ETL Pipeline Preparation.ipynb
                |-- ETL_Preparation.db
                |-- messages.csv
                |-- ML Pipeline Preparation.ipynb
          |-- README}
          
Installation
Here are the different packages used for this project:

- Numpy, Pandas, Sklearn
- NLTK
- SQLalchemy
- Flask, Plotly
After you've installed and imported all the necessary packages, you can run the program by following the steps below!

Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

   To run ETL pipeline that cleans data and stores in database python data/process_data.py data/disaster_messages.csv 
   data/disaster_categories.csv data/DisasterResponse.db
   
   To run ML pipeline that trains classifier and saves python models/train_classifier.py data/DisasterResponse.db 
   models/classifier.pkl

2. Run the following command in the app's directory to run your web app. python run.py

3. Go to http://0.0.0.0:3001/


