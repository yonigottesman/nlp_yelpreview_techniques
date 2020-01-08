Different techniques and frameworks to solve sentiment of the YelpReviewPolarity dataset.
https://www.yelp.com/dataset/challenge

## fasttext 
https://fasttext.cc/  
Parameters as used in https://github.com/facebookresearch/fastText/blob/master/classification-results.sh

## SimpleNN
Simple neural network implemented in pytorch.  
word embeddings -> avarage on words -> fully connected

## fastai  
https://www.fast.ai/  
Defaults and used like in docs

## Current results:

| model        | precision     | train time [mm:ss]|
| ------------- |:-------------:| :-------------:|
| fasttext      |     0.956          |    00:26     |
| SimpleNN      |       0.94        |     03:47 |
| gru      |       0.962        |     08:00 |
| bi-lstm * 2      |       0.967        |     25:00 |
|  fastai      |               | |
|  BERT      |               | |
