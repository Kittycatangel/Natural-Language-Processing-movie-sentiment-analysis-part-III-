# Natural Language Processing Movie Sentiment Analysis (PartIII)

# Introduction

This is based on the first two parts of Natural Language Processing Part I and II. The notebook of python code cn be found in this repository as Untiltled.iypnb

# Advanced Tokenization, Stemming, and Lemmatization

As mentioned previously, the feature extraction in the CountVectorizer and Tfidf Vectorizer is relatively simple, and much more elaborate methods are possible. One particular step that is often improved in more sophisticated text-processing applications is the first step in the bag-of-words model: tokenization. 

Lemmatization and stemming, are forms of normalization that try to extract some normal form of a word.

Stemming is always restricted to trimming the word to a stem, so “was” becomes “wa”, while lemmatization can retrieve the correct base verb form, “be”. Similarly, lemmatization can normalize “worse” to “bad”, while stemming produces “wors”.


# Latent Dirichlet Allocation

Intuitively, the LDA model tries to find groups of words (the topics) that appear together frequently. LDA also requires that each document can be understood as a “mixture” of a subset of the topics. It is important to understand that for the machine learning model a “topic” might not be what we would normally call a topic in everyday speech, but that it resembles more the components extracted by PCA or NMF, which might or might not have a semantic meaning.

We will learn another model, this time with 100 topics. Using more topics makes the analysis much harder, but makes it more likely that topics can specialize to interesting subsets of the data:

![image](https://user-images.githubusercontent.com/53411455/147393160-7deb5d85-7854-404d-9be7-14607c1f71ef.png)


# Conclusion

We talked about the basics of processing text, also known as natural language processing (NLP), with an example application classifying movie reviews. The tools discussed here should serve as a great starting point when trying to process text data.

In particular for text classification tasks such as spam and fraud detection or sentiment analysis, bag-of-words representations provide a simple and powerful solution. As is often the case in machine learning, the representation of the data is key in NLP applications, and inspecting the tokens and n-grams that are extracted can give powerful insights into the modeling process.

In text-processing applications, it is often possible to introspect models in a meaningful way, as we saw in this chapter, for both supervised and unsupervised tasks. You should take full advantage of this ability when using NLP-based methods in practice.
