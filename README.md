# Text Classification using naive bayes
Predicting Amazon ratings based on reviews by Text Classification using the Naive Bayes Algorithm.

## Name
naive - Run the executable program for Naive Bayes

## Synopsis
`./naive <part> <tr> <ts> <output>`

## Description
This program will train naive bayes model using given code on train data, make
predictions on test data and write final predictions in given output file.

## Options
- **PART**

  Part i.e. a,b or c
- **TR**

  File containing training data in csv format where 1st entry is the target
- **TS**

  File containing test data in csv format where 1st entry is the target
- **OUT** 

  Output file (write your predictions in this file)

## Example
`./naive a train.csv test.csv output`

### Parts

- **Part A**
    - Used Unigrams as features
    - Used Laplace Smoothing to avoid zero probabilities(c = 1)
    - Used Logarithms to avoid underflow issues
    - Implemented everything from the First Principles and not usde any existing R/python modules.

- **Part B**
    - All in Part A plus some Pre-Processing
    - Stopword Removal(nltk)
    - Stemming(nltk)
    - String Cleaning
  
- **Part B**
    - Feature Engineering
    - Lemmatization
    - Used Bigrams as features

## Data
- amazon_train.csv: Train data
- amazon_test_public.csv: Public Test data

Note: In the Public test data, actual class labels are replaced with -1

