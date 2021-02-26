## Starbucks Capstone Challenge

The capstone project represents an experiment in Starbucks that was carried out for a period of one month. The insight that we are after is: what next? More specifically, we want to have a proper customer segmentation. Certain kinds of people will represent to certain offers in different ways.

Some of the questions that are of interest to us include:
- What are the various types of customers in the data?
- How attractive is each individual offer, and to which type of customers?


### Data Sets
The data is contained in three files:

- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
- profile.json - demographic data for each customer
- transcript.json - records for transactions, offers received, offers viewed, and offers completed
Here is the schema and explanation of each variable in the files:

#### portfolio.json

- id (string) - offer id
- offer_type (string) - type of offer ie BOGO, discount, informational
- difficulty (int) - minimum required spend to complete an offer
- reward (int) - reward given for completing an offer
- duration (int) - time for offer to be open, in days
- channels (list of strings)

#### profile.json

- age (int) - age of the customer
- became_member_on (int) - date when customer created an app account
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
- id (str) - customer id
- income (float) - customer's income

#### transcript.json

- event (str) - record description (ie transaction, offer received, offer viewed, etc.)
- person (str) - customer id
- time (int) - time in hours since start of test. The data begins at time t=0
- value - (dict of strings) - either an offer id or transaction amount depending on the record



### Libraries
- numpy
- pandas
- matplotlib.pyplot
- seaborn


## How to run the analysis:
Start with the EDA directory, files are ordered numerically. Each stage uses the data generated from previous steps.
