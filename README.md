# Page Rank and Recommendation Systems
![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white)

We used the Scikit-learn and SciPy frameworks, in particular the SciKit Network and SciKit Surprise libraries, to perform PageRank (also Topic specific and personalized) and build a Recommendation System.

For the PageRank it has been used a Harry Potter related dataframe while for the recommendation part it has been used a user-item utility matrix where the utility has been expressed as ratings.

## Page Rank

#### Topic Specific Page Rank
In **topic-specific PageRank** we want to limit the probability distribution used by the algorithm to only those pages that are related to a certain **topic**.

#### Personalized Page Rank
In personalized PageRank we want to limit the probability distribution used by the algorithm to only one page.

#### Online-computation of Topic-specific PageRank given the single Personalized PageRank vectors
To speed up the calculation of Topic-specific PageRank in an online context, it is possible to calculate offline the personalized PageRank of all nodes belonging to the topic and then aggregate the results.

## Recommendation Systems

#### Basic Methods

  * Normal Predictor
  
  * Baseline Only
  
#### Neighborhood Methods

* KNNBasic: A basic collaborative filtering algorithm.

* KNNWithMeans: A basic collaborative filtering algorithm, taking into account the mean ratings of each user/item.

* KNNWithZScore: A basic collaborative filtering algorithm, taking into account the z-score normalization of each user/item.

* KNNBaseline: A basic collaborative filtering algorithm, taking into account a baseline rating.

#### Matrix Factorization-based Methods

* SVD 

* SVD++

### Hyper Parameters Optimization

“A hyperparameter is a parameter whose value is set before the learning process begins. By contrast, the values of other parameters are derived via training.” wikipedia.

Surprise offers two different methods for tuning the hyper parameters:

  * Grid Search Cross-Validation (exhaustive search)

  * Randomized Search Cross-Validation (randomized search)
