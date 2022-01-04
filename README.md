# Jedha_nlp_disasters_tweet
Text analysis and prediction with deep learning
NLP - or Natural Language Processing - is shorthand for a wide array of techniques designed to help machines learn from text. Natural Language Processing powers everything from chatbots to search engines, and is used in diverse tasks like text classification, sentiment analysis and machine translation.


## **Goal to be achieved**
The goal is to build 
- conduct exploratory data analysis (EDA) of the the dataset
- a machine learning model that predicts which Tweets are about real disasters and which ones are not.


## **General considerations**
In the EDA notebook, special attention has been brought to the production of the graphs with the packages stylecloud.
cf figure below of the disasters keywords frequence

![image](https://user-images.githubusercontent.com/32369680/148103223-87014e83-edf0-41e1-91a9-ef5ab744a70a.png)

or this wordcloud with unknown topic

![image](https://user-images.githubusercontent.com/32369680/148103460-fa02c4ec-0c2a-4948-97bf-62a2e9341745.png)

Scattertext is an elegant, interactive tool to elevate text analysis
'''@article{kessler2017scattertext,
  author    = {Kessler, Jason S.},
  title     = {Scattertext: a Browser-Based Tool for Visualizing how Corpora Differ},
  booktitle = {Proceedings of ACL-2017 System Demonstrations},
  year      = {2017},
  address   = {Vancouver, Canada},
  publisher = {Association for Computational Linguistics},
}'''


{{< figure src="https://drive.google.com/file/d/1-nG7SExgWTAdL2f9u10Wxqvv2l7Nudro/view?usp=sharing" title="Tweets scattertext" >}}
 https://htmlpreview.github.io/?https://drive.google.com/file/d/1-nG7SExgWTAdL2f9u10Wxqvv2l7Nudro/view?usp=sharing

We proove that the words, keywords and hashtags contained in each tweet are a good indicator of whether they're about a real disaster or not (They are !)


## **Results**
The models built with Google Sentence Encoder or Transformers have the great advantage of not requiring any particular preprocessing, unlike the sequential models. 

The best validation accuracy has been reached with Google Sentence Encoder (0.84176)

![image](https://user-images.githubusercontent.com/32369680/148094069-0069dd23-5392-4c6e-9df7-e811a0a19aed.png)

Concerning the sequential model, I was quite impressed to discover that early stopping allowed to save a model with a val_accuracy equal to 0.80789.

![image](https://user-images.githubusercontent.com/32369680/148096182-29ac31d7-85cd-47a2-90bb-7423e8755c89.png)



## **Conclusion **


I hope in the future to deepen my basic understanding of these tremendously complex techniques (...)
