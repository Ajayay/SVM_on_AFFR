
### Amazon Fine Food Reviews Sentiment Analysis.

This dataset is taken from kaggle.com

### For conceptual understanding you can refer : 
        https://medium.com/@ajayphroust.ay/support-vector-machines-svm-c9ef22815589
### Objective:
- The main goal of the project is to analyze some large dataset and perform sentiment classification on it. Sentiment classification is a type of text classification in which a given text is classified according to the sentimental polarity of the opinion it contains. For the purpose of this project the Amazon Fine Food Reviews dataset, which is available on Kaggle, is being used.

- Following sections describe the important phases of Sentiment Classification: the Exploratory Data Analysis for the dataset, the preprocessing steps done on the data, learning algorithms applied and the results they gave and finally the analysis from those results.

### Context:
1. This dataset consists of reviews of fine foods from amazon. 
2. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. 
3. Reviews include product and user information, ratings, and a plain text review. 
4. It also includes reviews from all other Amazon categories.

### Dataset link https://www.kaggle.com/snap/amazon-fine-food-reviews.

- Number of reviews: 568,454
- Number of users: 256,059
- Number of products: 74,258
- Timespan: Oct 1999 - Oct 2012
- Number of Attributes/Columns in data: 10

### Data includes:
 - Reviews from Oct 1999 - Oct 2012
 - 568,454 reviews
 - 256,059 users
 - 74,258 products
 - 260 users with > 50 reviews


### Feature information:

- IdRow Id
- ProductIdUnique identifier for the product
- UserIdUnqiue identifier for the user
- ProfileNameProfile name of the user
- HelpfulnessNumeratorNumber of users who found the review helpful
- HelpfulnessDenominatorNumber of users who indicated whether they found the review helpful
- ScoreRating between 1 and 5
- TimeTimestamp for the review
- SummaryBrief summary of the review
- TextText of the review

### Text preprocessing techniques used:
- BOW
- TFIDF (simply replace the BOW  preprocessing technique by TFIDF at every place.)

### Models used:
1. SVM (classification)

### Preparing data for model:
1. Numerical Conversion: 
- SVM assumes that you have inputs are numerical instead of categorical. So you can convert them using one of the most commonly used "one hot encoding , label-encoding etc".
2. Binary Conversion:
- Since SVM is able to classify only binary data so you would need to convert the multi-dimensional dataset into binary form using (one vs the rest method / one vs one method) conversion method.

### Unlike in previous models we would not be using for loop for hyperparameter tunning instead we will be simply using GridsearchCV function.


