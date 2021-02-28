# Probably Interesting Data

The main goal fo this project is to implement mixture models without using default Machine Learning Libraries and apply the models on two datasets.

## Datasets:
For this project, I have used datasets from UCI ML kaggle repositories. Below are the links for the datasets. These datsets can be found in the Data sub folder.

1. [Auto Mpg Dataset](https://www.kaggle.com/uciml/autompg-dataset)
2. [PIMA Indians Diabetes Datset](https://www.kaggle.com/uciml/pima-indians-diabetes-database)

## Algorithms:
For this project, I have implemented the following two algorithms:

1. K Means algorithm
2. Expectation Maximization algorithm

## Explanation:
The implementation for these algorithms are located in the Notebooks folder.

### K means:
k means function takes the dataset, variables needed for the calculations and k value for the clusters, the plot is drawn initially before the dataset is clustered. Initial centroids are taken randomly, later the points are compared with closest centroid and assigned to the respective cluster. This loop continues until the distance becomes zero between new and old centroids.

For the first auto mpg dataset, I implemented k means clustering in order to model the data. Auto mpg dataset is taken from the performance of various car models. Based on the data analysis, I observed that weight vs mpg and acceleration vs mpg depict a good distribution of data based on the plots drawn. I used these features further and applied the k means algorithm on these features. From the plots, we can clearly see the differentiation between the clusters for each of them. K means algorithm worked pretty well on this dataset and successfully seperated the two clusters.

### Expectation Maximization:
The EM mixture model is used to develop a univariate guassian mixture model. It has two steps, which are called as E and M steps respectively. In E step we will give initial values to mu, sigma, pi and calculate the latent variable for all instances. In M step we will update the values of the same and do the convergence test. The convergence test is fnding the difference between previous adn updated values and if the difference is less than 0.01 they are converged.

I have used EM mixture model on PIMA Indians Diabetes dataset, this dataset describes the features responsible for getting diabetes. Here, based on the features graphs are drawn initially, and they were not pure guassian models but later after applying EM mixture model, we can see the pure guassian distribution for each feature respectively.

## Steps to execute:
1. Download the files from the github repository.
2. Get the diabetes.csv and auto-mpg.csv file by unzipping the .zip file.
3. Place the csv files in datasets folder and place the datasets folder in notebooks folder. The notebooks folder should also have ipynb file as well.
4. Navigate to terminal and type "jupyter notebook"
5. Navigate to the folder where the notebooks are placed.
6. From the menu icon cell, select the notebook and click on Run all which will run the whole notebook from the first cell.

## Steps to follow:
1. Set up a new git repository in your GitHub account
2. Pick two datasets from https://www.kaggle.com/uciml/datasets
3. Choose a programming language (Python, C/C++, Java)
4. Formulate ideas on how machine learning can be used to model distributions within the dataset
5. Build a heuristic and/or algorithm to model the data using mixture models of probability distributions programmatically
6. Document your process and results
7. Commit your source code, documentation and other supporting files to the git repository in GitHub

### References:
https://towardsdatascience.com/implement-expectation-maximization-em-algorithm-in-python-from-scratch-f1278d1b9137 </br>
http://www.aishack.in/tutorials/expectation-maximization-gaussian-mixture-model-mixtures/ </br>
https://mubaris.com/posts/kmeans-clustering/ </br>
https://machinelearningmastery.com/expectation-maximization-em-algorithm/ </br>

