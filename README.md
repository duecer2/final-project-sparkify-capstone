# Udacity-Data-Scientist-Capstone-Sparkify
## Welcome to my Capstone in python
### [Medium](https://ebenite2.medium.com/utilizing-k-means-clustering-to-determine-churn-rates-of-music-subscription-users-in-pyspark-ed0ebbf70991)

There are two jupyter notebooks to satisfy the requirements of this capstone project.  As the data is extremely large for a local instance, and my IBM cluster utilized all lite instances; I had to split the notebooks into two.  The first notebook is merely an exploratory phase, to understand the data, and to gain insights for how to compute the purpose of churn rates.  While the notebooks are related and utilize the same dataset, the library requirements do differ slightly.  Due to professional considerations, the dataset, and vectorized model data will not be published to github.

Libraries required:

* os, sys, requests
* pandas, numpy
* plotly, matplotlib
* pyspark

Motivation for the captsone outside the realm of completing the project requirements include, a lifelong desire to merge mathematics, and computer science in an applicable, and industrious way.  As technology has taken hold, it is machine learning which seems to satisfy this niche pursuit in a more than satisfactory way.

Github project consists of the following,
    
    jupyter notebook -- sparkify_capstone.ipynb:
    -----------------------------------------------
         * The jupyter notebook of python code used in numerical calcualtions.
         
    jupyter notebook -- exploratory analysis.ipynb:
    -----------------------------------------------
         * The jupyter notebook utilized for exploratory analysis.
 
    markdown -- README.md:
    ----------------------
         This markdown holds various information on the github repository.  My basic solution of the initial dataset were threefold,
            1.  Pysparks Machine Learning API requires vectorization
            2.  The data sets contains non numerical values, given this and the large data size, Pipeline is:
                    * StringIndexer => VectorAssembler => StandardScaler => ChiSqSelector => kMeans 
            
