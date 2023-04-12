# Sentiment-Analysis-on-Movie-Reviews
### Transformers for Sentiment Classification

### **Description**
The project that the proposal infers to is called [Movie Review Sentiment Analysis](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/overview). The main goal is to classify the sentiment of reviews from the Rotten Tomatoes dataset. The Rotten Tomatoes movie review dataset is a corpus of movie reviews used for sentiment analysis. The main task is to label phrases on a scale of five values: negative, somewhat negative, neutral, somewhat positive, positive. There are many obstacles such as sentence negation, sarcasm, language ambiguity, and many others make the sentiment prediction more difficult. In general, this particular Sentiment Analysis is a multiclass classification task to be faced.

In the project I will show you in detail how to implement four types of well-known transformer models making use of the transformers HuggingFace library and Keras API. 


### **Data**
The main task corresponds to a multi-class text classification on Movie Reviews Competition and the [Dataset](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/data) contains 156,060 instances for training, whereas the testing set contains 66,292 from which we have to classify among 5 classes.

The sentiment labels are:

- 0 → Negative
- 1 → Somewhat negative
- 2 → Neutral
- 3 → Somewhat positive
- 4 → Positive

At the end of the project we will summarize and compare their performance according to our requirements and metrics. 

### **Modeling**
In this step we will build, train and compare the following algorithms:

- BERT (Bidirectional Encoder Representation from Transformers)
- RoBERTa (Robustly Optimized BERT Pre-training Approach)
- DistilBERT (Distilled BERT)
- XLNet (Generalized Auto-Regressive model)

Each one of the mentioned have its pros and cons, the most preferred and widely used model is the BERT for being the middle term in performance, whereas RoBERTa and .. are known for their better error metrics and DistilBERT for its faster training. We will consider all of these chracteristics and choose the best one for our dataset.

Firstly, we have to install the transformers library offered by HuggingFace so as enable all useful functions when building the four models.

In summary the performance of the four models was similar, supporting the idea that BERT is the middle term of trade-off between accuracy and training time, whereas DistilBERT was the fastest by far, but having a lower accuracy than the previous as is explained by HuggingFace it achieves 95% accuracy of BERT, finally RoBERTa and XLNet were the models with highest accuracy and at the same time the slowest.
