# Recommender System Overview
During the last few decades, with the rise of Youtube, Amazon, Netflix, and many other web services, recommender systems have taken more and more place in our lives. A recommender system is a subclass of information filtering systems that seeks to predict the "rating" or "preference" a user would give to an item. Recommender systems are utilized in various areas, including movies, music, news, social tags, and products in general. Recommender systems typically produce a list of recommendations in one of two ways – through collaborative filtering or content-based filtering.

### Collaborative Filtering
Collaborative methods for recommender systems are based on the past interactions recorded between users and items to produce new recommendations. These interactions are stored in the so-called "user-item interactions matrix."

### Content-based Filtering

Unlike collaborative methods that only rely on user-item interactions, content-based approaches use additional information about users and/or items.  This approach utilizes a series of discrete characteristics of an item to recommend other items with similar properties.

### Hybrid Recommender
This one combines the previous two approaches.

## Movie Recommender System Development

I've started my project with content based recommendation system and implemented it in 2 different ways:
  1. Cosine similarity based
  2. Euclidean distance based
