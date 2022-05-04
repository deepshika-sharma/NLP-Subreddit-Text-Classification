# Reddit Post Classification and NLP

## Problem Statement
Company XYZ is planning to create a platform for streaming movies. The company wants to know which movies to stream or not depending on the box office posts from Reddit.
The company would like to know if a particular post/comment is from the box office subreddit or not so that they can later analyze it further to understand which posts are positive about a movie and which are not.



## Executive Summary
This project focuses on Reddit posts classification, mainly figuring out which subreddit a post or comment belongs to through the use of Natural Language Processing (NLP) techniques.

The data was collected using the [PushShiftAPI](https://github.com/pushshift/api) in conjunction with a wrapper called [pmaw](https://github.com/mattpodolak/pmaw) which enables the ability to collect large amounts of data which might not be possible with the API alone.
The data collected was then cleaned and preprocessed using NLP tools like the WordNetLemmatizer.

Models which were used to evaluate the data were Logistic Regression, Decision Trees Classifier, Support Vector Classifier(SVC), Multinomial Naive Bayes and Random Forest Classifier.



## Data
The data was collected from the subreddit boxoffice(r/boxoffice) and movies(r/movies)

### Data Dictionary
Collected from Reddit using the API and wrapper.

| Column | Description|
|--------|------------|
|author| Name of the author of the post|
| author_fullname | author ID |
| permalink | URL of the post |
| title | Title of the post |
| body | content of the comment |
| selftext | content of the post |


## Conclusion and Recommendations
The models produced similar scores upon evaluation which was about 76%. As the subreddits overlap more it is more harder for the model to give good evaluations. 
More hyperparameter tuning can be carried out to see if there are any changes to the evaluation metrics.
For further analysis, sentimental analysis of the posts and comments can be carried with a Sentimental Analyzer tool like Vader to figure out whether a post/comment is positive, negative or neutral. 
This can help the company better their services for their clients.