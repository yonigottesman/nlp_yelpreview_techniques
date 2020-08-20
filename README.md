Different techniques and frameworks to solve sentiment of the YelpReviewPolarity dataset.
https://www.yelp.com/dataset/challenge

## fasttext 
https://fasttext.cc/  
Parameters as used in https://github.com/facebookresearch/fastText/blob/master/classification-results.sh

## SimpleNN
Simple neural network implemented in pytorch.  
word embeddings -> avarage on words -> fully connected

## rnn
Some rnn networks inplemented in pytorch.
gru, bi-lstm

## tfidf
sklearn tfidf + logistic

## bert
Fine tuning the whole bert model with an additional linear layer.  
To save money (google cloud run time...) I use only 100K train examples.  
To fit in gpu memory i use only 128 tokens (long examples get cut).



## Current results:

| model        | precision     | train time [mm:ss]|
| ------------- |:-------------:| :-------------:|
| fasttext      |     0.956          |    00:26     |
| SimpleNN      |       0.94        |     03:47 |
| gru      |       0.962        |     08:00 |
| bi-lstm * 2      |       0.967 |     25:00 |
|  tfidf      |        0.939       |    00:16 |
|  **BERT** - fine tuning      |   ###            |224:00|
