# Yelp Data Analysis

## Abstract

In this project, our team analyzed the Yelp Challenge Dataset. We explored the review distribution and discovered that majority of reviews are composed of 4-star and 5-stars, reflecting that a user's feedback is, in general, optimistic towards a business after receiving the service. We found that the imbalance of 4-star and 5-star reviews in the dataset are consistent in terms of geographical decomposition. Nine cities receiving most reviews all exhibit the imbalance of 4-star and 5-star reviews in the dataset. 

Following exploratory data analysis, we applied Natural Language Processing techniques. After some preprocessing steps, including removing stop words and tokenizing words, we converted the corpus of all user reviews to a data matrix, in which each entry is a value, or TF-IDF statistics. TF-IDF, or term frequency-inverse document frequency, statistics is intended to reflect the importance of a word in the corpus. In our context, TF-IDF is the indication of how much a word contributes to the rating of a user review. We used multinomial Naive Bayes and multi-class Support Vector Machine to predict user ratings. The overall accuracy is 0.52 and 0.6, respectively. 

These results suggest that a better modeling approach should be considered when predicting user ratings based on user reviews. Merely using 1-gram (i.e. words) does not yield satisfactory outcome. This might be due to the length of user reviews. The correlation between user rating and user review should be considered, bacause user reviews are short on average. One alternative is to use bigram to build the model. 
