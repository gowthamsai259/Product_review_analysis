# Product_review_analysis
There are various columns in the product rating analysis in which some columns are useless for the analysis part.
As this dataset is almost having 23000+ rows there will be obviously some missing values in some columns.
I have tried to remove the null values but during the analysis I have faced some errors.
So I have decided to use "ffil" method to eliminate the null values in the data.

In the rating column the rating is written in terms of words. So I have extracted the rating out of five as a number.
I have found the Unique products(using .unique()) which is useful to calculate the overall rating of each product.

Finally after doing all these, I have decided to read the sentiment of the reviews in which we have to use NLP(nltk library).
But nltk is not exactly working in my system. So I have decided to use TextBlob(pip install textblob) in which it is used to determine the polarity of the sentence.
Based on the polarity, we can decide that the sentence is positive or negative or neutral.
For example, if the sentence polarity is greater than '0', then its a positive sentence and negative for less than '0' and neutral for '0'.
Finally a column was added to tell that review is positive or negative or neutral.
