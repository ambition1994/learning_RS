* Recommender systems are replacements of search engines by reducing the efforts in proactive searches and surprising users with offers they never searched for.

### Three task
1. how to predict the rating a user might give to a prospective item
2. how to generate a recommendation list of items
3. how to predict the click-through rate from abundant features


Recommendation System -> Powerful information filtering tool


### Benefits of RS
* largely reduct users' effort in finding items and alleviate the issue of information overload
* add business value to online service providers and is an important source of revenue

### Collaborative Filtering
* memory based CF
	* user based CF
	* item based CF
	* limitations: dealing with sparse and large scale data, since it computes the similarity values based on common items.
* model based CF : matrix factorization, neural CF(extend, use deep learning)
* hybrid CF
* Only user user-item interaction data to make predictions and recommendations. While there also are content-based, context-based recommendation system

explicit feedback (less data, many users may be reluctant to rate products)
implicit feedback: user click, purchase history, browsing history

### Recommendation Tasks
* domain of applications
* types of feedback and input data
* cold-start recommendation: 
	recommending for new users and recommending new items to existing users