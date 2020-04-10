# Disaster_Response_Pipeline-DSND


![Intro Pic](screenshots/intro.png)

## Table of Contents
1. [Description](#description)
2. [Getting Started](#getting_started)
	1. [Dependencies](#dependencies)
	2. [Installing](#installing)
	3. [Executing Program](#executing)
3. [Authors](#authors)
4. [Acknowledgement](#acknowledgement)
5. [Screenshots](#screenshots)

<a name="descripton"></a>
## Description

This Project is part of Data Science Nanodegree Program by Udacity in collaboration with Figure Eight.
The initial dataset contains pre-labelled tweet and messages from real-life disaster. 
The aim of the project is to build a Natural Language Processing tool that categorize messages.

The Project is divided in the following Sections:

1. Data Processing, ETL Pipeline to extract data from source, clean data and save them in a proper databse structure
2. Machine Learning Pipeline to train a model able to classify text message in categories
3. Web App to show model results in real time. 

<a name="getting_started"></a>
## Getting Started

<a name="dependencies"></a>
### Dependencies
* Python 3.5+ (I used Python 3.7)
* Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
* Natural Language Process Libraries: NLTK
* SQLlite Database Libraqries: SQLalchemy
* Web App and Data Visualization: Flask, Plotly

<a name="installing"></a>
### Installing
Clone this GIT repository:
```
git clone https://github.com/buchan123/Disaster-Response-Pipeline.git
```
<a name="executing"></a>
### Executing Program:
Note: Run the above commands on a cmd prompt or linux terminal in the local git directory.
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database(Just Pass the parameters)
        `python3 data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python3 models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python3 run.py`

3. Go to http://0.0.0.0:8000/


<a name="authors"></a>
## Authors

* [Mayukh Sil](https://github.com/mayukhsil)

<a name="acknowledgement"></a>
## Acknowledgements

* [Udacity](https://www.udacity.com/) for providing such a great and complete course for learning Data Science.
* [Figure Eight](https://www.figure-eight.com/) for providing the dataset to train my model

<a name="screenshots"></a>
## Screenshots

1. This is an example of a message you can type to test Machine Learning model performance

![Sample Input](screenshots/sample_input.png)

2. After clicking **Classify Message**, you can see the categories which the message belongs to highlighted in green

![Sample Output](screenshots/sample_output.png)

3. The main page shows some graphs about training dataset, provided by Figure Eight

![Main Page](screenshots/main_page.png)
