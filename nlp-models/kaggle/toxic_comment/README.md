The task is to [Identify and classify toxic online comments](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)

Please install two more libraries:
* nltk
* gensim
* tqdm

My solution is to train three models and then ensemble:
```
cd model_gru
python train.py

cd model_lstm
python train.py

cd model_tfidf_lr
python train.py

python ensemble.py
```