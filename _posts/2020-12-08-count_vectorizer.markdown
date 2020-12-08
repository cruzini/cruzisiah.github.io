---
layout: post
title:      "Count Vectorizer"
date:       2020-12-08 13:45:38 -0500
permalink:  count_vectorizer
---


**Overview**

This specific blog will focus on the Count Vectorizer — a useful tool that that counts the number of times that a word appears across a set of text documents. By creating a matrix with each row representing a document and each column representing unique words in the document, the Scikit-Learn package is a quick way to separate every word in a document into vectors (aka a list of numbers).

**Examples of Count Vectorizer**

**1) Raw text before Count Vectorizer:**

"For every 100,000 inhabitants, Okinawa has 68 centenarians — more than three times the numbers found in U.S. populations of the same size"

Count Vectorizer results:

 
**2) Raw text before Count Vectorizer:**

"The Okinawan way is to do all things in moderation. As you eat, practice mindfulness by listening to your body"

Count Vectorizer results:
 

**3) Raw text before Count Vectorizer:**

"Older Okinawans adopt a plant-based diet, with their meals mostly consisting of stir-fried beans, spinach, mustard greens, sweet potatoes and tofu — all of which are high in nutrients"

Count Vectorizer results:
 

**What Count Vectorizer Does**
As shown in the examples above, Count Vectorizer creates a unique vector for every word in a text document (i.e. 'adopt' is vector 0, 'potatoes' is vector 20) and then shows how many times each word shows up in an array (i.e. vector 0 shows that the word 'adopt' only showed up once). 

**Code for Stopwords**

1. Import the necessary packages

2. Import your text documents

3. Create an initializer for the Count Vectorizer

4. Fit the desired text document with your vectorizer
 
5. Visualize the different vectors created for each word

6. Encode the vector

7. Display the results of Count Vectorizer in array form

**Conclusion**

The Count Vectorizer is much the opposite of the TF-IDF Vectorizer, which is a relatively robust weighting system that takes into account the number of times that a word appears in a document (rewarding frequency) and how unique a word is across documents (rewarding originality). Instead, the Count Vectorizer is a straightforward way to derive meaning from text documents by measuring only the number of times that a word appears.

**Sources**
* https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html
* https://kavita-ganesan.com/tfidftransformer-tfidfvectorizer-usage-differences/#.X8unLRNKglU
* https://stackoverflow.com/questions/49618950/using-countvectorizer-to-compute-word-occurrence-for-my-own-vocabulary-in-python
* https://www.geeksforgeeks.org/using-countvectorizer-to-extracting-features-from-text/
* https://towardsdatascience.com/hacking-scikit-learns-vectorizers-9ef26a7170af
* https://www.quora.com/What-is-the-difference-between-TfidfVectorizer-and-CountVectorizer-1
* https://www.educative.io/edpresso/countvectorizer-in-python
* https://www.cnbc.com/2020/11/10/japanese-80-percent-diet-rule-can-help-you-live-longer-says-longevity-expert.html

