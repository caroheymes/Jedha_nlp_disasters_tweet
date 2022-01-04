## **Foreword : nlp & deep learning for text classification**

Text analysis and prediction  NLP (Natural Language Processing) or deep learning is shorthand for a wide array of techniques designed to help machines learn from text. Natural Language Processing powers everything from chatbots to search engines, and is used in diverse tasks like text classification, sentiment analysis and machine translation.

## **Goals to be achieved**
The goal is to :
- conduct exploratory data analysis (EDA) of the the dataset
- build a machine learning model that predicts which Tweets are about real disasters and which ones are not.

## **General considerations**
In the EDA notebook, special attention has been brought to the production of the graphs with the packages stylecloud. 

cf figure below 
Tweets related with disasters plot :

![image](https://user-images.githubusercontent.com/32369680/148109207-e2ec4d64-65ba-4b2f-80f7-48505e52ba07.png)


Unknown topic tweets main words :

![image](https://user-images.githubusercontent.com/32369680/148109296-dd0c6403-9a61-4ec8-ac66-2d27d4287d0b.png)

Scattertext is an elegant, interactive tool to elevate text analysis 
```@article{kessler2017scattertext, author = {Kessler, Jason S.}, title = {Scattertext: a Browser-Based Tool for Visualizing how Corpora Differ}, booktitle = {Proceedings of ACL-2017 System Demonstrations}, year = {2017}, address = {Vancouver, Canada}, publisher = {Association for Computational Linguistics}, }```
Please see the map in the notebook
![scattertext](https://user-images.githubusercontent.com/32369680/148113942-f3ada51f-29f0-4519-9c88-9aef30ec9315.png)


We proove that the words, keywords and hashtags contained in each tweet are a good indicator of whether they're about a real disaster or not (They are !)

## **Results**
The models built with Google Sentence Encoder or Transformers have the great advantage of not requiring any particular preprocessing, unlike the sequential models.

The best validation accuracy has been reached with Google Sentence Encoder (0.84176)

![image](https://user-images.githubusercontent.com/32369680/148117368-b048890b-2b1d-4bb7-9416-f4eaf6452c13.png)


Concerning the sequential model, I was quite impressed to experience that early stopping allowed to save a model with a val_accuracy equal to 0.80789.



## **Perspectives**
I need in the future to deepen my basic understanding of these tremendously complex techniques (...)
