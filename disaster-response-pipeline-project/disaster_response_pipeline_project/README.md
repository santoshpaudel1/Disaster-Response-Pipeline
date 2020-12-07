# Disaster Response Pipeline Project
In this project, it is analyzed disaster data from Figure Eight to build a model for an API that classifies disaster messages. The data set contains real messages that were sent during disaster time. A ETL and machine learning (ML) pipeline is created to categorize these events so that one can send the messages to an appropriate disaster relief party.

The project also includes a web app where an emergency worker can input a new message and get classification results in fidderent categories

Project Link: https://github.com/santosh13579/disaster-response-pipeline-project/tree/main/disaster-response-pipeline-project/disaster_response_pipeline_project

File Descriptions:

    ETL Pipeline Preparation.ipynb: Notebook experiment for the ETL pipelines
    ML Pipeline Preparation.ipynb: Notebook experiment for the machine learning pipelines
    data/process_data.py: The ETL pipeline used to process data in preparation for model building.
    models/train_classifier.py: The Machine Learning pipeline used to fit, tune, evaluate, and export the model to a Python pickle
    app/templates/~.html: HTML pages for the web app.
    run.py: Start the Python server for the web app and prepare visualizations.


### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/
