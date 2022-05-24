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


---

# Disaster Response Pipeline Project

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
	`cd app` , then `python run.py`
    or `python app/run.py

3. Open another terminal and type `env|grep WORK` this will give you the spaceid (it will start with view*** and some characters after that)
	Now open your browser window and type `https://viewa7a4999b-3001.udacity-student-workspaces.com`, 
    replace the whole `viewa7a4999b` with your space id that you got in the step 2
	Press enter and the app should now run for you

4. on Local Machine once your app is running (python run.py)

5. Go to http://0.0.0.0:3001/
