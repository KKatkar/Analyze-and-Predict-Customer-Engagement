# Stabucks_Capstone_Challenge
**Problem Statement:**
To explore, analyse and identify the best offer that will ensure prolonged customer engagement with the Starbucks brand. These tasks will be performed on simulated datasets that mimics the data of the actual Starbucks rewards application. The final model will be able to determine whether an offer will generate a response or not from the customer.

**Notebook Files:**
The Data Exploration, Data wrangling and Feature Engineering phases are in the Starbucks_Capstone_Notebook.ipynb file and the modelling and evaluation phases are in the Modeling.ipynb file.

**Datasets: (provided by Starbucks)**
portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
profile.json - demographic data for each customer
transcript.json - records for transactions, offers received, offers viewed, and offers completed

Structure:
_portfolio.json_
•	id (string) - offer id
•	offer_type (string) - type of offer ie BOGO, discount, informational
•	difficulty (int) - minimum required spend to complete an offer
•	reward (int) - reward given for completing an offer
•	duration (int) - time for offer to be open, in days
•	channels (list of strings)

_profile.json_
•	age (int) - age of the customer
•	became_member_on (int) - date when customer created an app account
•	gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
•	id (str) - customer id
•	income (float) - customer's income

_transcript.json_
•	event (str) - record description (ie transaction, offer received, offer viewed, etc.)
•	person (str) - customer id
•	time (int) - time in hours since start of test. The data begins at time t=0
•	value - (dict of strings) - either an offer id or transaction amount depending on the record

**Installation:**
Python 3.x 
Python libraries: NumPy
		  Pandas
		  Matplotlib – plot graphs
		  Sklearn
		  Json – to read data files
		  Scipy – to generate distriutions
		  Pprint

**Reflection:**
In this project I successful created a Machine Learning model to tackle the challenge of identifying the conversion of an offer successfully. I successful wrangled and explored the data to understand the distributions and trends of the customer base. I was able to observe the patterns of offer distribution by Starbucks. 
I was able to evaluate our model against the benchmark model and justify the selection of the best model. Then the models hyperparametes was tuned and performance was evaluated. The model performed well over unseen data with an accuracy of 91% and F1 score of 91%.


