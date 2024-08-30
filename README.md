# Sentiment_Analysis_Reviews_Charlotte_NC_Restaurants
Used Python (Tokenization, Stemming and WordCloud) to prepare and visualize reviews of Charlotte, NC restaurants. Developed LDA topic model and classified a 14,000+ text corpus into key topics/labels using R-Studio with Radiant. Analyzed and obtained actionable insights from the observed results: sentiment score, review count, topics, and ratings.

## Overview
The project is essentially about text analysis. The text of customer reviews of Charlotte, NC restaurants were analyzed using a combinationation of programs and processes:

1. Python was use to ultimately generate a word cloud. The original body text were prepared using python pre-processing techniques such as tokenization and stemming.

2. Topic Modeling to sieve through the text and tease out semantic similarity and coherence.

3. Regression Model - All numerical variables have been log transformed to smooth out the outliers/extreme values and to dampen the effect of observations with zero values.

4. Analyses and Drawing Insights - The relationships between Sentiments Score, Review count, Topics, and Ratings are captured and reviewed.

5. Conclusion.

## Word Cloud

5 main themes were revealed: good, food, place, great, and service. These words are indicating that the dominant theme is about restaurants, about great food, and emotional and passionate the clients feel to comment. Joyous and positives predominate in the word cloud. To a restaurant business in the Charlotte area, this should be of interest, as the message coming across is that a good location, good food and great service can deliver a competitive edge, in a fairly crowded terrain.
<img width="327" alt="image" src="https://github.com/user-attachments/assets/600af2d7-cb1f-4b0a-a596-1b6dc247bda9">

## Topic Modeling

Latent Dirichlet Allocation (LDA) topic model was employed in selecting the number of topics to focus on. In determine the label for each topic, I have sense checked the theme running through each topic that also set each of them, to some extent, apart from the other ones. In the topics table below, the wining label, by and large, summed up the other words in the topic. 10 topics was chosen due to the dimension of the dataset – over 14,000 text corpus by several restaurants. After a few iterations, 10 topics felt about right.
<img width="468" alt="image" src="https://github.com/user-attachments/assets/c3739805-6c3f-4a3d-88f7-ece843dc6d7a">

The view is also presented in a chart format. Each topic consists of 20 words. Although some words such as food, good, and place are present in more than one topic (they are also prominent in the word cloud), the topics that fall under and other associated terms are suggest a high level of semantic similarity and coherence.
<img width="468" alt="image" src="https://github.com/user-attachments/assets/f2144d11-24e7-4b29-bbcc-002ea74228c4">

## Regression Model
<img width="468" alt="image" src="https://github.com/user-attachments/assets/3de57f98-5e9b-4473-8a09-7976ec68f6c1">

The model is indicating that ‘joy’ has a positive relationship with ratings, in contrast to ‘disgust’ that shows an influence but in the opposite direction.

### Model Fit/Reliability: 
20.6% of the variability in rating is explained by the model. This is reflected in the R-squared of 0.206. The adjusted R-squared of the same number, 0.206 is indicating the absence of irrelevant variables in the model.
The high F-statistic value  of 457.7 and low p-value 0.00 suggest that at least one independent variable significantly contributes to predicting the rating, the dependent variable.

Three emotion variables, appear not have any statistically significant impact on the variability in ratings. Surprise, fear, and anger all have p-values greater than 0.05 that is typically considered the threshold for statistical significance. Of the ones that are statistically significant, joy shows the highest impact at 27.7%. This is indicating that joy increases rating by 28% for every unit of joy expressed. Disgust has the next highest impact on rating, but a negative one. Disgust is indicating that there is a circa 19% decrease in rating when 1 unit of disgust is expressed.

Trust, sadness, and anticipation all have relatively small negative impacts on ratings when they are expressed in customer reviews. Joy, disgust and trust are the top three emotions that can predict the ratings. The overall 20.6% of changes in ratings that is connected to emotions is suggesting that there are factors at play that influence customers ratings of the restaurant businesses in Charlotte.

## Analysis and Drawing Insights

The relationships between Sentiments Score, Review count, Topics, and Ratings are captured in a table. Restaurant open vs. close status is also reflected in the chart.
<img width="468" alt="image" src="https://github.com/user-attachments/assets/bf99c26e-7f7e-4d12-999b-6bab867c3d8e">

There are some evidence that may support the argument that restaurants with higher ratings may have higher number of review. For example, higher reviews, ratings, and sentiments tend to go hand in hand. Topic 2 – Friendly had highest average total reviews, ratings, and sentiments scores. Open restaurants show significantly higher average reviews score than restaurants with close status. I have called out three topics to support this: topics 1 (breakfast/brunch), 3 (light food), and 6 (timely service).

## Conclusion

The significance of the text analysis for sentiment and emotion, is indicating that the topics of the reviews are related to the ratings. Friendly, good food, and a nice location resonate with customers and move them to express joyous emotions. The metrics could point a restauranter in focus area in Charlotte to the fact that, although there may other strong factors in play, that are not captured in this excercise, positives emotions expressed by the consumers can be leveraged to hone their service quality. 
