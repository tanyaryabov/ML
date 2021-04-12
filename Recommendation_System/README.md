# Recommender System Overview
During the last few decades, with the rise of Youtube, Amazon, Netflix, and many other web services, recommender systems have taken more and more place in our lives. A recommender system is a subclass of information filtering systems that seeks to predict the "rating" or "preference" a user would give to an item. Recommender systems are utilized in various areas, including movies, music, news, social tags, and products in general. Recommender systems typically produce a list of recommendations in one of two ways – through collaborative filtering or content-based filtering.

### Content-based Filtering
The content-based approach requires a good number of items’ features rather than user interactions and feedback. For example, it can be movie attributes such as genre, year, director, actor, etc. This approach utilizes a series of discrete characteristics of an item to recommend other items with similar properties.

### Collaborative Filtering
Collaborative methods for recommender systems are based on the past interactions recorded between users and items to produce new recommendations. These interactions are stored in the so-called "user-item interactions matrix."

### Hybrid Recommender
This one combines the previous two approaches.

# Movie Recommender System Development

I've started my project with content based recommendation system and implemented it in 2 different ways:
  1. [Cosine similarity based](https://github.com/tanyaryabov/ML/blob/master/Recommendation_System/Content_Based_Netflix_Recommender.ipynb)
  2. [Euclidean distance based](https://github.com/tanyaryabov/ML/blob/master/Recommendation_System/Content_Based_Netflix_Recommender__euc_sim.ipynb)
  
Then moved to two classes of Collaborative Filtering:  
  1. [User-based, which measures the similarity between target users and other users](https://github.com/tanyaryabov/ML/blob/master/Recommendation_System/RS_collaborative_filtering_user_based.ipynb)
  2. [Item-based, which measures the similarity between the items that target users rate or interact with and other items](https://github.com/tanyaryabov/ML/blob/master/Recommendation_System/RS_collaborative_filtering_item_based.ipynb)

Implementation of Hybrid recommender:
  1. [Hybrid recommendation system](https://github.com/tanyaryabov/ML/blob/master/Recommendation_System/Hybrid_recommendation_system.ipynb)
  
 Model based recommendation system:
  1. [KNN]
  2. [SVD]

### Movie Recommendation Engine Development with KNN:

Collaborative filtering Item-based approach is usually preferred than the user-based approach. A user-based approach is often harder to scale because of the dynamic nature of users. In contrast, items typically don't change much, so an item-based approach can often be computed offline.
KNN is a perfect go-to model for this use case, and KNN is a very good baseline for recommender system development. In item-based collaborative filtering, KNN will use a pre-defined distance metric to find clusters of similar items based on users' ratings and make recommendations using the distance metric in item ratings of top-k nearest neighbors.

#### Let's Make Some Recommendations:
"Pulp Fiction" is one of my favorite movies so I want to test what 5 movies recommendations my system is giving me:

<p>Output:</p>
<p>Movie Selected:  Pulp Fiction (1994)</p>
<p>Silence of the Lambs, The (1991)</p>
<p>Shawshank Redemption, The (1994)</p>
<p>Seven (a.k.a. Se7en) (1995)</p>
<p>Forrest Gump (1994)</p>
<p>Usual Suspects, The (1995)</p>

### Movie Recommendation Engine Development with SVD:
