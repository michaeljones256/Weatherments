# Weatherments

### Weatherments is a software that combines analyisis of tweet setniments using NLTK and weather sentiments using a homergrown mapping from weather data to degrees of goodness to figure out the general mood of people in a specific area during certain weather states.
<br />

### Hunter Malley, Hong Chen, Mike Jones, Robert Robinson, Julia Barucky

<br />

## Before running our program we have to install some dependencies:
    
     Start by installing all of the python packages required:
        1. open directory Weatherments
        2. "pip install -r requirements.txt" in command prompt and the neccesary packages will be delivered
        **** Warning: you might have to explicitly install the scipy file as follows:
            "pip install scipy"

     Then we have to download the required NLTK corpora:
        1. in the directory Weatherments 
        2. "python Req.py" in command prompt and the necessary corpora will be downloaded
        ***NOTE: this my take a moment to finish dowloading

## Now that all of our dependencies are installed:

     Our Python module TweetCollector.py uses Cookbook.py functions to stream tweets based on location, where their 
        sentiment is analyized and the current weather sentiment is assinged. Each tweet collected is then sent to our database
        
        *** We kindly ask that if you run this module, please comment out line 22 'print(DB.saveToDB(i))' so our databse is not mutated

        To run this module enter 'python TweetCollector.py'  into the command line


     Our Python module Alalysis.py displays our findings from our data. 
        To run this module enter 'python Analysis.py' into the command line.

     Our Python module Classifier.py contains our Bayes Classifier that is fed a small set of tweets 
        and outputs the type of day it thinks it was created on.

     To view our dataset that we have collected, you can open the file DataFile.json