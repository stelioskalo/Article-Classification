# Article Classification
This project is related to the Project found in Improov-Admin-UI repository. The goal of the project was to train different machine
learning algorithms in order to be able to classify the category (topic) of newly added articles.

The folders are numbered between 1 and 5 which indicate which programs were developed and used first before moving to the next ones.

## 1. Article Retrieval and Dataset Creation
I have not found a dataset online that would serve my exact purpose so I decided to create one myself. I had manually collected
a number of URLs containing business articles and labeled them appropriatly using 21 classes.

Once I had all URLs and their labels, I created a Web Scraper program using python were all the "p" elements found in the URL were retrieved (articles).
Once retrieved, all articles were saved in a CSV file containing 1287 rows.

The folder contais the CSV file as well the ipynb program.

## 2. Data Analysis
This section of the project performs an exploratory data analysis of the dataset. The analysis constists of plotting a graph displaying 
the number of articles in each category as well as their percentages, the length of each category and box plots. The graphs help
visualise the dataset to get a better view on how to process it.

## 3. Features Engineering
Since there are no features yet extracted, this part of the project extract the features from each sample. For this project TFIDF vectors
were used. Features Engineering consisted of; text cleaning (e.g. special character cleaning, upcase/downcase, lemattization etc.), label
codification, splitting the dataset to training and testing and creation of the TFIDF vectors.

## 4. Model Training
This section is concerned with the training of different machine learning algorithms using the extracted features. A number of different 
machine learning algorithms were trained in order to decide which had the best accuracy to use in the application. The algorithms
used were; Random Forest, Support Vector Machine, K-nearest neighbour, Multinomial Naive Bayes and Multinomial Logistic Regression. Three
different cross-validation techniques were used for all models for hyper parameter tuning. The best model for each machine learning algorithm
was saved.

## 5. Best Model Selection
Code was written in order to plot a graph showing each model's accuracies. That help to identify which one had the highest accuracy in order
to use in the application.

## Technologies Used
Python

BeautifulSoup

Pandas

Matplotlib

Pickle

Altair

Nltk

Scikit-learn

Numpy

Tensorflow

## How to Run
Google Colab would be the most ideal to run the project, but other notebooks would do the trick as well.
Note that file paths will need to be changed.
