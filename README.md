# uML[PCA, Clustering(KMean,AHC)]

A PCA is undertaken on the USArrests dataset to reduce the datasets dimensionality. Then KMeans and Agglomerative Hierarchical Clustering are implemented on the PCA dataset. The dataset used contains crime statistics per 100,000 and the percentage of urban population for each state . Scikit-learn was used for the clustering algorithms.

## Description 

The dataset is pre-processed to identify missing values, view the distribution of the features and the datatypes are explored. 

A PCA is undertaken on the raw data initially with an accopamning bo-plot to display how unscaled data can impact your results. The data is then scaled used StandScalar. 

After this another PCA is perfomed to investigated and determine the optimal number of features needed to explain atleat 80% of the variance in the dataset.  Multiple correlation matrices and a bi-plot are used to determine which features are influences which PCs. 

The KMeans model is trained using the selected PCs to determine the optimal amount of clusters. Once this is determined by using the Elbow method and calculating the silhoutte scores for a range of K values identified from the Elbow Method. The K value with the highest silhoutte score is selected as K. 

The optimum value for K is then used in the AHC model, in which scatterplots and dendrograms of different distance metrics and linkages are used to determine which metrics are best. A scatterplot with the optimum metrics at the selected K value is plotted and clusters interpreted. 
