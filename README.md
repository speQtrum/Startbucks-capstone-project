# Starbucks Capstone Project
Capstone Project in Data Scientist Nanodegree of Udacity

## Project Motivation<a name="motivation"></a>

It is the Starbuck's Capstone project of the Data Scientist Nanodegree in Udacity. We get the dataset from the program that creates the data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers. We want to make a recommendation engine that sends personalized offers to customer.

We are interested to answer the following two questions:
1. Which offer should be sent to a particular customer to let the customer buy more?
2. Which demographic groups respond best to which offer type?


## Files <a name="files"></a>


The data is contained in three files:
- `portfolio.json` - containing offer ids and meta data about each offer (duration, type, etc.)
- `profile.json` - demographic data for each customer
- `transcript.json` - records for transactions, offers received, offers viewed, and offers completed





## Results and Findings<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@joshua.chyeung/send-out-a-starbucks-offer-that-you-cannot-resist-2d4d7d18b417).

Based on the transcript records, we build an user-item-matrix that represents how users responded to the offers they received. We then split the records into the training set and the test set and trained our SVD algorithm to predict how a user responses to a particular offer. We achieved the lowest mean square error around 0.003823 with 15 latent features with the training set and around 0.009175 with 10 latent features with the testing set. After that, we created a recommendation engine that recommends Starbucks which offer should be sent to a particular user.

In the later section, we found out which demographic groups respond best to which offer type. Female respond much better than men, in both BOGO and discount. Men react slightly better to discount than BOGO. We also found that it is better to promote the offer via social media. Among the ten offers, sending buy 10 dollars get 2 dollars off within 10 days offer via email, web, mobile and social makes Starbucks gain more. It is the best offer so far!


## Licensing, Authors<a name="licensing"></a>

Thanks to Starbucks for the data.
