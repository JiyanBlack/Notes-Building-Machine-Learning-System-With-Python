# Clustering

* Problem: recommend the related articles to one article.

* Steps:
  1. Turn raw text into numerical features, use edit distance. 
    * Wrong way: two words "machine" and "machien" needs at least two edits to turn one to the other. We treat the whole article as a vocabulary and one word as a character.
    It doesn't take the reordering into account. Time complexity is high.
    * Right way: bag-of-word approach. Count the occurency of each word in the article, recorded into a vector.
