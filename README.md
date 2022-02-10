# DisasterResponsePipelines
model that classifies disaster messages for an API built from disaster data sourced on Figure Eight


Here's the file structure of the project:

- app
  - template
  - master.html  # main page of web app
  - go.html  # classification result page of web app
  - run.py  # Flask file that runs app

- data
  - disaster_categories.csv  # data to process 
  - disaster_messages.csv  # data to process
  - process_data.py
  - InsertDatabaseName.db   # database to save clean data to

- models
  - train_classifier.py
  - classifier.pkl  # saved model 

- README.md