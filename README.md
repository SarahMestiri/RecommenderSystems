# Recommender Systems
## Introduction
This repository contains resources about Recommender Systems as well as my RecSys projects trying out different methods.

**Do you know that recommendation engine knows you better than you best friend?** 

Amazon, Netflix, Zalando, and many other companies are providing each customer a personalized user experience through recommendations. These recommendations fit the customer's interests. That means, if you are a software engineer, then Amazon will suggest programming books for you, and if you are a new mom, then it will suggest baby toys, diaper,etc. 
The magic of recommender systems is more than that: they not only ***provide you with what you need***, but also ***surprise you with things that you didn't know you will like***!

**How is this unique "You" leveraged by recommender systems?**

Let's discover that by learning more about one of the most famous methods for recommender systems: *Collaborative Filtering (CF)*!

Note: If you want to get an idea about the different types of recommender systems. check this article [5 Types of Recommenders](https://www.datasciencecentral.com/profiles/blogs/5-types-of-recommenders).

## Collaborative Filtering 
The basic idea behind collaborative filtering is that people who agreed in certain evalution patters in the past, are likely to agree again in the future.

### Memory-based Collaborative Filtering
Memory-based collaborative Filtering is one of the earliest methods developed for collaborative filtering, it's also called, Neighborhood-based collaborative filtering. We can distinguich 2 primary types in neighborhood methods:
1. **User-based** collaborative filtering:<br>
   Similar users are considered to have similar ratings on the same item.
2. **Item-based** collaborative filtering:<br>
   Similars items are considered to have similar ratings by the same user. <br>

Neighborhood-based methods can be viewed as generalizations of k-nearest neighbor classifiers (KNN).

Although both types (user-based & item-based) have similar results, Item-based CF is often preferred because it uses the user's **own** ratings. Besides, it's more stable with changes => adding new user occurs more than adding new item => more similarity calculations and update of the ratings matrix.
### Model-based Collaborative Filtering

Model-based Collaborative Filtering are more advanced methods that are considered more effective than memory-based collaborative filtering. They offer space-efficiency and they able to deliver accurate results even with a sparse matrix.

Some of the most accurate methods used in recommender systems are based on model-based techniques in general, and one of the most effective methods among them is **latent factor models**.

#### Latent Factor Models
Latent Factor Models leverage dimensionality reduction methods in order to estimate the ratings matrix. It uses the fact of high correlation between rows and columns of the ratings matrix which results in the approximation by a ***low-rank matrix*** and it's possible to obtain the fully specified low-rank matrix because of the redundancies in the data, even with a smaller subset of the original ratings matrix.

A good explanation of Matrix Factorization used by Latent Factor Models in order to reduce the dimension of the matrix is [here](http://nicolas-hug.com/blog/matrix_facto_1) by Nicolas Hug, Surprise Library developer.

### Building a recommender system using collaborative filtering (with Resources)

To build a recommender system, you have a large set of libraries that you can use, and each one of them has its advantages and drawbacks.
You can find a good Quora answer about the topic here:

* [What is the best open source package to build a recommender system with Python - Quora](https://www.quora.com/What-is-the-best-open-source-package-to-build-a-recommender-system-in-Python/answer/Xavier-Amatriain?srid=hpTX9)

Start with a small dataset then scale it to see what's the difference between results. Also, because if you choose a big dataset it's possible to get a MemoryError like it happened to me when I used the whole dataset of book-crossing. To scale the dataset, I would suggest to use Spark as it has a strong performance.

* [Implementation of movie recommendations using Neighborhood methods - Python and Scikit-Learn](http://blog.ethanrosenthal.com/2015/11/02/intro-to-collaborative-filtering/)
* [Implementation of movie recommendations using ALS and SGD - Python and Scikit-Learn](http://blog.ethanrosenthal.com/2016/01/09/explicit-matrix-factorization-sgd-als/)
* [Implementation of movie recommendations - Spark & Flask ](https://www.codementor.io/jadianes/building-a-recommender-with-apache-spark-python-example-app-part1-du1083qbw)
* [Deploying Machine Learning Models in production as APIs](https://www.analyticsvidhya.com/blog/2017/09/machine-learning-models-as-apis-using-flask/)
* [Recommender Systems through Collaborative Filtering - Implementation with Surprise Lib](https://blog.dominodatalab.com/recommender-systems-collaborative-filtering/)

### Available Datasets

* [Recommendation and Ratings Public Data Sets For Machine Learning](https://gist.github.com/entaroadun/1653794)
* [The nine must have datasets for investigating Recommender Systems](https://gab41.lab41.org/the-nine-must-have-datasets-for-investigating-recommender-systems-ce9421bf981c)

## Reference
* **Recommender Systems -The Textbook** by Aggarwal, Charu C.
* [Customers expect personalized recommendations - salesforce report 2016](https://www.salesforce.com/blog/2017/07/customers-expectations-in-age-of-the-customer.html)

## Note
Originally I gave this as a talk in [Data Natives](www.datanatives.io) 2017. Slides are [here](https://www.slideshare.net/secret/ihqcoDDwkSQrAo)
