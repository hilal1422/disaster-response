# Disaster Response Pipeline

### Summary of project
This udacity data science nano degree project. Purpose of this project is to correctly classify the disaster request into 3 predefined categories. This porject has three parts - ETL pipeline this is to extract data from csv file, clean it, and store it in sqlite database - ML pipeline I used multi lable classifier to correctly classify message in one or more than one of predefined 36 categories - web application Flask based web application to display result

The web app also displays visualizations of the data.

## Web application screenshots

![file1](https://github.com/Kusainov/udacity-disaster-response/blob/master/file1.JPG)

![file2](https://github.com/Kusainov/udacity-disaster-response/blob/master/file2.JPG)

![file3](https://github.com/Kusainov/udacity-disaster-response/blob/master/file3.JPG)

### Technologies Used
•	Python
     o	Libraries: pandas, sklearn, sqlite3, sqlalchemy, nltk, plotly, flask
•	HTML
    o	Bootstrap

### Run
1.	Run the following commands in the project's root directory to set up your database and model.
o	To run ETL pipeline that cleans data and stores in database python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db
o	To run ML pipeline that trains classifier and saves python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl
2.	Run the following command in the app's directory to run your web app. python run.py
3.	Go to http://0.0.0.0:3001/


### Data observations
As can be seen from test data visualization most of the classes (categories) are highly imbalanced. This affects model F1 prediction score. One using this project should take this into consideration and apply measures like synthetic data generation, model selection and parameters fine-tuning, etc.     
