# Song-Genre-Classifier

## Steps followed

## Data Cleaning
1.Apply NLTK word tokeniser<br/>
2.Make all terms lower case<br/>
3.Substitute regular expressions with spaces<br/>
4.NLTK stop words are commonly used words, coming from nltk.corpus, a dump of NLP datasets. Remove those frm the dataset<br/>
5.Stemming : producing morphological variant of root/base word<br/>
### Types of stemming :
* Porter  :plural/-ing/-ion/-ed/many of these [Used in this project]<br/>
* Snowball : a better version, English stemmer/porter2 stemmer<br/>
* Lancaster : sometimes causes overstemming<br/>
* Regexp :we construct the obects,where we pass the regular expressions, and substrings matching regular expressions are discarded<br/>


## Data Analysis and Visualization
1.Find the mean word count per genre for all songs in that group<br/>
2.Plot word cloud for each genre<br/>

## Feature Extraction - TFIDF Vectorization

Tfidf Vectorization 
* Term frequency is the number of occurrences of a term in the document<br/>
* Every text from data is represented as a matrix whose rows are the number of documents, columns are number of distinct terms throughout all documents<br/>
* Document frequency is the number of documents containing a specific term<br/>
* Idf: log(n/df), the weight of the term ; idfi is the idf score for term i, n is the total number of documents<br/>

Now, train the Multinomial Naive bayes classifier model on the computed tfidf scores, we have 11 categories.

## Working of Naive Bayes Algorithm
1. Calculates probability for each tag, gives highest one as output<br/>
2. Works on the condition that each feature used in classification is independent of the other<br/>

Bayes Theorem 
```
P(A|B)=A(B|A)*P(A)/P(B)
```

## Evaluation metrics 
* Recall 
* Precision 
* Accuracy 
* F1score 






