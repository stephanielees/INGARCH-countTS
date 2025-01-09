# INGARCH-countTS
INGARCH process for count time series

The demo video is [here](https://youtu.be/89e2Nley1uo)

Discrete time series can be found in many applications, and the nature of such time series is different from the continuous time series. Therefore, we need a different way to find the best process that could generate count time series. Integer-valued GARCH (INGARCH) is one of various models for modelling (nonnegative) discrete time series.

What's in this repository?
 1. `datasource-wikipedia-math.ipynb`: This is the notebook describing how I got the original data, which is time series of graphs (more technically, it's called a spatiotemporal type of data), and extract the data from one node.
 2. `wiki_BucketSort.csv`: The output of the file above. This csv file contains the time series of Bucket Sort in Wikipedia and of the pages which mention Bucket sort (the covariates).
 3. `CountTS-INGARCH.Rmd`: The main file.

I initially wanted to use Python for all the steps in this project. In fact, I tried using another model that I studied first before INGARCH. But I got stuck in the coding stage 😅, so I changed my plan (for now) to using INGARCH, which has many implementation packages written in R.
