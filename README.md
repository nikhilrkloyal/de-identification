# De-identification model for PHI/PII 

## Setup:

Requires Python 3.9

Set up requirements using:

`pip install -r requirements.txt`


Setup spaCy model used by presidio-analyzer 

`python -m spacy download en_core_web_lg`


## About:
This project utilises token classification using HuggingFace transformer models to identify PHI/PII information in text utterances.
The goal is to be able to use this model to detect and mask patient sensitive information from chatbot queries. The model currently supports 
the following classes:

+ Person/Name
+ Geopolitical Entity (City, State, Country)
+ Organization/Company
+ Date/Time
+ Street Address
+ Credit Card Number
+ Title (Mr., Mrs., etc)
