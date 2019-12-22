# MSDS 696: Practicum II
## Emma Highland

## Background
This project uses the [MovieLens 100k Dataset](https://grouplens.org/datasets/movielens/100k/). Below I have included the citation for this data set.

> F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets:
History and Context. ACM Transactions on Interactive Intelligent
Systems (TiiS) 5, 4, Article 19 (December 2015), 19 pages.
DOI=http://dx.doi.org/10.1145/2827872

For this project, I performed exploratory data analysis and data cleaning in R (see associated .Rmd file). One step I took was to limit the genres included, using only genres that appeared a minimum of 10,000 times. Because individual movies are classified into multiple genres, this did not eliminate any movies. I chose to eliminate some more rare genres in order to obtain unique results, as I planned to follow a tutorial that used all data.

In this notebook, I use the K-Nearest Neighbors algorithm for two different purposes. First, I implement a KNN approach to suggest movies based on a given movie as a reference point. For this step, I follow the example of M. Hendra Herviawan, available for your consideration at [this link](https://hendra-herviawan.github.io/Movie-Recommendation-based-on-KNN-K-Nearest-Neighbors.html). Second, I implement a KNN approach using the library scikit-learn. The purpose of this second use of KNN was to predict genre from ratings. 

Overall, my goal is to examine the recommendations and consider how the different features of the dataset might inform the recommendations.

## Results

My goal was to examine the recommendations and consider how the different features of the dataset might inform the recommendations.

My major take aways from this analysis are:
* The tutorial KNN implementation is fairly successful as is
* The amount of genres used in the dataset has a larger influence on which movies are recommended than the ratings do
* Rating and genre do not have a strong relationship
