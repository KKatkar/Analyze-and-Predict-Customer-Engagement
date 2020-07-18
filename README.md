# Stabucks_Capstone_Challenge<br />
<h2>Problem Statement:</h2><br />
To explore, analyse and identify the best offer that will ensure prolonged customer engagement with the Starbucks brand. These tasks will be performed on simulated datasets that mimics the data of the actual Starbucks rewards application. The final model will be able to determine whether an offer will generate a response or not from the customer.

<h2>Notebook Files:</h2><br />
The Data Exploration, Data wrangling and Feature Engineering phases are in the Starbucks_Capstone_Notebook.ipynb file and the modelling and evaluation phases are in the Modeling.ipynb file.

<h2>Datasets:</h2> (provided by Starbucks)**<br />
portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)<br />
profile.json - demographic data for each customer<br />
transcript.json - records for transactions, offers received, offers viewed, and offers completed<br />

<h2>Structure:</h2><br />
_portfolio.json_<br />
•	id (string) - offer id<br />
•	offer_type (string) - type of offer ie BOGO, discount, informational<br />
•	difficulty (int) - minimum required spend to complete an offer<br />
•	reward (int) - reward given for completing an offer<br />
•	duration (int) - time for offer to be open, in days<br />
•	channels (list of strings)<br />

_profile.json_<br />
•	age (int) - age of the customer<br />
•	became_member_on (int) - date when customer created an app account<br />
•	gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)<br />
•	id (str) - customer id<br /><br />
•	income (float) - customer's income

_transcript.json_<br />
•	event (str) - record description (ie transaction, offer received, offer viewed, etc.)<br />
•	person (str) - customer id<br />
•	time (int) - time in hours since start of test. The data begins at time t=0<br />
•	value - (dict of strings) - either an offer id or transaction amount depending on the record<br />

<h2>Installation:</h2><br />
Python 3.x <br />
**Python libraries:**<br /> NumPy,<br />
		  Pandas,<br />
		  Matplotlib – plot graphs,<br />
		  Sklearn,<br />
		  Json – to read data files,<br />
		  Scipy – to generate distriutions,<br />
		  Pprint<br />

<h2>Reflection:</h2><br />
In this project I successful created a Machine Learning model to tackle the challenge of identifying the conversion of an offer successfully. I successful wrangled and explored the data to understand the distributions and trends of the customer base. I was able to observe the patterns of offer distribution by Starbucks. 
I was able to evaluate our model against the benchmark model and justify the selection of the best model. Then the models hyperparametes was tuned and performance was evaluated. The model performed well over unseen data with an accuracy of 91% and F1 score of 91%.


