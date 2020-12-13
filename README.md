# fragrance-clustering
K-means++ clustering on fragrance accords

<img src="https://img.shields.io/badge/python-3.8.2 -brightgreen"> <img src='https://img.shields.io/badge/scikitlearn-0.23.2-blue'> <img src='https://img.shields.io/badge/pandas-1.1.1-blue'> <img src='https://img.shields.io/badge/numpy-1.19.1-blue'> <img src="https://img.shields.io/badge/yellowbrick-1.1 -blue"> <img src="https://img.shields.io/badge/matplotlib-3.3.1 -blue"> <img src="https://img.shields.io/badge/seaborn-0.10.1 -blue"> <br>
<img src="https://img.shields.io/badge/unsupervised-machine--learning-ff69b4"> <img src="https://img.shields.io/badge/cluster-analysis-ff69b4"> <img src="https://img.shields.io/badge/exploratory-data%20analysis-ff69b4">

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)
* [Screenshots](#screenshots)
* [Status](#status)

## General info
Unsupervised machine learning project with K-Means++ clustering performed on different female fragrances.

This project is part of my fragrance exploration series:
1. K-means++ clustering on fragrance accords <br>
https://github.com/katarzynajanicka/fragrance-clustering
2. Agglomerative hierarchical clustering on 39.7K female fragrances <br>
https://github.com/katarzynajanicka/agglomerative-fragrance-clustering
3. Accords-based recommendation system for female fragrances <br>
https://github.com/katarzynajanicka/fragrance-finder

## Technologies
Project is created with Python - version: 3.8.2.

Python libraries:
* scikit-learn - version 0.23.2
* pandas - version 1.1.1
* numpy - version 1.19.1
* yellowbrick - version 1.1
* matplotlib - version 3.3.1
* seaborn - version 0.10.1
  
## Setup

Input data: perfume.csv, source: https://www.kaggle.com/sagikeren88/fragrances-and-perfumes

Output data: fragrances.ipynb

## Screenshots

**Objectives**

![](./screenshots/objective.png)

**Project structure**

![](./screenshots/content.png)

## Results

**Data structure**

![](./screenshots/columns.png)

![](./screenshots/df.png)

**Data exploration**

![](./screenshots/rating.png)

![](./screenshots/accord.png)

![](./screenshots/splitaccords.png)

![](./screenshots/fragrancefamily.png)

**Choosing the right number of clusters**

![](./screenshots/elbow.png)

![](./screenshots/elbowviz.png)

![](./screenshots/silhouette.png)

![](./screenshots/silhouette4.png)

![](./screenshots/silhouette6.png)

![](./screenshots/silhouette10.png)

![](./screenshots/silhouette14.png)

![](./screenshots/silhouette19.png)

**Four fragrance clusters**

![](./screenshots/4clusters.png)

![](./screenshots/4clustersindata.png)

**Most popular fragrances**

![](./screenshots/mostpopular.png)

**Conclusions**

Clustering, like other unsupervised machine learning algorithms, is very exploratory in nature.

The weakness of the K-means algorithm (and its optimized K-means++ version deployed in this analysis) is the need to determine the number of clusters in advance. However, additional metrics such as distortion used in the elbow method or silhouette coefficient may be helpful in choosing the number of clusters a priori. The number of clusters should be primarily determined based on the business needs.

Cluster descriptions show the general, average characteristics of the members of a given cluster (cluster centroids). One cluster may share the same characteristics with other clusters. On the basis of the analyzed data, the division into four categories of perfumes (fresh, floral, oriental and woody) turned out to be the most accurate.

Agglomerative hierarchical clustering technique may be a more correct approach as the different perfumes have a large overlap in fragrance accords. Perfume fragrances usually have the same notes, although they belong to different fragrance families.

## Status
Project completed.
