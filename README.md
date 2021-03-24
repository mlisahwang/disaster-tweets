# Kaggle's Natural Language Processing with Disaster Tweets Competition
### March 24, 2021
### Lisa Hwang
### https://www.kaggle.com/c/nlp-getting-started


### Objective
To practice natural language processing (NLP) and predictive modeling by entering Kaggle's Disaster Tweets competition.


### Repo Contents
- README.md
- preds.csv - Disaster tweet predictions that were submitted to Kaggle
- DisasterTweetsNotebook.ipynb - Jupyter Notebook for modeling


### Competition Description From Kaggle
>"Twitter has become an important communication channel in times of emergency.
The ubiquitousness of smartphones enables people to announce an emergency they’re observing in real-time. Because of this, more agencies are interested in programatically monitoring Twitter (i.e. disaster relief organizations and news agencies).

>In this competition, you’re challenged to build a machine learning model that predicts which Tweets are about real disasters and which one’s aren’t. You’ll have access to a dataset of 10,000 tweets that were hand classified. If this is your first time working on an NLP problem, we've created a quick tutorial to get you up and running."


### Data
The ```train.csv``` and ```test.csv``` were downloaded from https://www.kaggle.com/c/nlp-getting-started.


### EDA
There were 7,613 rows (or tweets) and 5 columns in the ```train.csv``` dataset. No null rows were present. Of most interest were the ```text``` column which was the actual tweet text and the ```target``` column which indicated if the tweet referred to an actual disaster or not (1 = yes, 0 = no). 


### Modeling: Logistic Regression
I decided to use ```LogisticRegression``` since it's a reliable and not-too-complicated method. After applying ```CountVectorizer``` with default parameters on the corpus, I got a training accuracy score of ```0.9702``` which was pretty respectable but a much lower testing score of ```0.8088```, indicating overfitting. I decided to go ahead and submit these predictions to Kaggle.


### Final Comments
This submission was originally uploaded to the competition on 12/3/20, and it received a score of ```0.79190```. With this entry, I became number 797 on the leaderboard out of 1338.
