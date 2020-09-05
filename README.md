# Reddit-post-popularity-prediction

Reddit is a popular social news website where users post their content with either links or text, which other users can "upvote" or "downvote". The amount of upvotes a post receives determines its popularity and thereby impacts its visibility on the website. A variety of factors play a great role in determining the popularity of a post.

The primary goal of this project is to develop a predictive machine learning model that will be able to predict the popularity of a post using various features from the post and its associated components. A training dataset of Reddit posts from the year 2006 is used to train the machine learning (ML) models. Even though the dataset was small enough to compute the computations on a single node, to explore and experiment with the principle of parallelism, the distributed systems in PySpark were used in the Databricks cluster.

The training dataset chosen was initially preprocessed and dealt with any missing values, outliers, and insignificant features. There were features with numerical, categorical as well as binary entries and each of them was dealt with independently. Later, features were explored using data visualization techniques and new features were engineered that helps in training the model. To optimize the computation time and cost and to reduce the model complexity, only important features were fed to the model.

Comparing the evaluation metrics like RMSE and R2, Random Forest Regressor was found to be the best model, delivering optimal results on both the test data and the out of time (OOT) datasets. Results on the OOT dataset were found to be in line with the results on the test dataset, confirming that the model is not overfitting. Since the input data was skewed, model performance on different bins was analyzed and it was concluded that the model is performing well on lower score posts as it could get enough training samples to learn from.

The future scope of this project includes building deep learning regressors for automating the feature selection process into the model and to obtain better results.
