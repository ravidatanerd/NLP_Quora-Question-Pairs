# NLP_Quora-Question-Pairs


PROJECT:	Natural Language Processing
	
Your work should be readable as well as correct. 

https://www.kaggle.com/c/quora-question-pairs/data


On this project
We are a two-members:

Ramesh Subedi

Ravi Dawar

"The goal of this competition is to predict which of the provided pairs of questions contain two questions with the same meaning. The ground truth is the set of labels that have been supplied by human experts. The ground truth labels are inherently subjective, as the true meaning of sentences can never be known with certainty. Human labeling is also a 'noisy' process, and reasonable people will disagree. As a result, the ground truth labels on this dataset should be taken to be 'informed' but not 100% accurate, and may include incorrect labeling. We believe the labels, on the whole, to represent a reasonable consensus, but this may often not be true on a case by case basis for individual items in the dataset.

Data fields
id - the id of a training set question pair
qid1, qid2 - unique ids of each question (only available in train.csv)
question1, question2 - the full text of each question
is_duplicate - the target variable, set to 1 if question1 and question2 have essentially the same meaning, and 0 otherwise. "

In general Quora uses a Random Forest model to identify duplicate questions.

Approach : Identify question pairs that have the same intent.

Can We ?
Yes we can capture the intent for the question and Compare them together to identify duplicates using LSTM .

But if we are using TF-IDF ,Count-Vectorizer It will not capture the intent but will only compare the Word Vector
and compare the Vector similarity , Which Is not apt technquie to use in our case. But Will implement it to figure the issues asssociated with these vectorizers.

We have Used the following for the analysis:
Quora’s train.csv file and Test.csv for Evalution 

Random Forest,
Support Vector,
XGBoost (Extreme Gradient Boosting) classifiers.

To Capture Sentiment Using:

word2vec embedding with MaLSTM (Manhattan Long Short-Term Memory) to capture sentiment.

