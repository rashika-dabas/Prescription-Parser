# Prescription-Parser

## Aim
Build a Doctor Prescription Parser with the help of CRF model

## Task
Build a Prescription Parser that takes a prescription (sentence) as an input and find / label the words in that sentence with one of the already pre-defined labels

## Problem
SEQUENCE PREDICTION - Label words in a sentence

## Input
Doctor Prescription in the form of a sentence split into tokens (Example: Take 2 tablets once a day for 10 days)

## Output
FHIR Labels
- ('Take', 'Method')
- ('2', 'Qty') 
- ('tablets', 'Form')
- ('once', 'Frequency')
- ('a', 'Period') 
- ('day', 'PeriodUnit')
- ('for', 'FOR')
- ('10', 'Duration')
- ('days', 'DurationUnit')

## Major Steps
- Install necessary libraries
- Import the libraries
- Create training data with labels
    - Split the sentence into tokens
    - Compute POS tags
    - Create triples
- Extract features
- Split the data into training and testing set
- Create CRF model
- Save the CRF model
- Load the CRF model
- Predict on test data
- Finding accuracy
