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
   
Although they both have similar results, Item-based CF is often preferred because it uses the user's **own** ratings. Besides, it's more stable with changes => adding new user occurs more than adding new item => more similarity calculations and update of the ratings matrix.
### Model-based Collaborative Filtering

### Building a recommender system using collaborative filtering (with Resources)

To build a recommender system, you have a large set of libraries that you can use, and each one of them has its advantages and drawbacks.
You can find a good Quora answer about the topic here:

* [What is the best open source package to build a recommender system with Python - Quora](https://www.quora.com/What-is-the-best-open-source-package-to-build-a-recommender-system-in-Python/answer/Xavier-Amatriain?srid=hpTX9)

[Recommender Systems through Collaborative Filtering - Implementation with Surprise Lib](https://blog.dominodatalab.com/recommender-systems-collaborative-filtering/)


### Available Datasets

* [Recommendation and Ratings Public Data Sets For Machine Learning](https://gist.github.com/entaroadun/1653794)
* [The nine must have datasets for investigating Recommender Systems](https://gab41.lab41.org/the-nine-must-have-datasets-for-investigating-recommender-systems-ce9421bf981c)
