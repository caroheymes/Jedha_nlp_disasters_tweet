Jedha_nlp_disasters_tweet
Text analysis and prediction  NLP (Natural Language Processing) or deep learning is shorthand for a wide array of techniques designed to help machines learn from text. Natural Language Processing powers everything from chatbots to search engines, and is used in diverse tasks like text classification, sentiment analysis and machine translation.

Goal to be achieved
The goal is to build

conduct exploratory data analysis (EDA) of the the dataset
a machine learning model that predicts which Tweets are about real disasters and which ones are not.
General considerations
In the EDA notebook, special attention has been brought to the production of the graphs with the packages stylecloud. cf figure below of the disasters keywords frequence

image

or this wordcloud with unknown topic

image

Scattertext is an elegant, interactive tool to elevate text analysis '''@article{kessler2017scattertext, author = {Kessler, Jason S.}, title = {Scattertext: a Browser-Based Tool for Visualizing how Corpora Differ}, booktitle = {Proceedings of ACL-2017 System Demonstrations}, year = {2017}, address = {Vancouver, Canada}, publisher = {Association for Computational Linguistics}, }'''



We proove that the words, keywords and hashtags contained in each tweet are a good indicator of whether they're about a real disaster or not (They are !)

Results
The models built with Google Sentence Encoder or Transformers have the great advantage of not requiring any particular preprocessing, unlike the sequential models.

The best validation accuracy has been reached with Google Sentence Encoder (0.84176)

image

Concerning the sequential model, I was quite impressed to discover that early stopping allowed to save a model with a val_accuracy equal to 0.80789.

image

**Conclusion **
I hope in the future to deepen my basic understanding of these tremendously complex techniques (...)
