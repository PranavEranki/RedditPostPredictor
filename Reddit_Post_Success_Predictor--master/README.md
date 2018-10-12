# Reddit Post Binary Success Predictor
Does tagging a Reddit post with "SPOILER" or "NSFW" correspond with more comments? What's the best time of the day to post content to maximize discussion? What subreddits command the most interaction?

This project is aimed at predicting whether or not an individual reddit post will garner user interaction, measured in unique user comments, in the upper quartile of the posts on Reddit's "Popular" page. 

In this pursuit I scraped Reddit using their native API to attain data on over 57,000 posts. I applied Natural Language Processing techniques to the title of the posts to engineer features highly correlated to a post's success or failure. Along with other post features I used scikit-learn to train three binary classification machine learning models.

# Model Accuracy on holdout data

Logistic Regression: 0.7544
	
	Regularization Penalty: Lasso
	Regularization Strength C: 0.01	

Random Forest Classifier: 0.7609
	
	max tree depth: None
	max tree features: 3
	n estimators: 40

Bagging Classifier: 0.7593
	
	n estimators: 10

Gradient Boosting Classifier: 0.7792
	
	max tree depth: 4
	max features: None
	n estimators: 100


	
