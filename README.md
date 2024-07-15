# Gaussian-Mixture-Models-GMM-
__Project Description__  
This repository focuses on understanding the use of Gaussian Mixture Models (GMM) for estimating mixture models, with a particular emphasis on choosing the number of components and the type of covariance matrix. The project involves both theoretical understanding and practical implementation using Scikit-learn functionalities.

__Core Components__
__1. Gaussian Mixture Models (GMM)__
GMM is a probabilistic model for representing the presence of subpopulations within an overall population. It assumes that all data points are generated from a mixture of several Gaussian distributions with unknown parameters.  
__2. Model Selection__  
Model selection involves choosing the number of mixture components and the type of covariance matrix. This can be done using the Akaike Information Criterion (AIC) or the Bayesian Information Criterion (BIC).
Key parameters include:  
•	n_components: Number of mixture components.  
•	covariance_type: Type of covariance matrix ('full', 'tied', 'diag', 'spherical').  
•	init_params: Method of parameter initialization ('kmeans', 'random').  
•	n_init: Number of initializations.  

3. Key Methods and Attributes
•	Methods:
o	fit(X): Compute the GMM parameters based on the data.
o	aic(X): Calculate AIC for the model.
o	bic(X): Calculate BIC for the model.
o	predict(X): Predict the labels for the data.
o	score_samples(X): Evaluate the log-likelihood of the data.
•	Attributes:
o	weights_: Mixture coefficients.
o	means_: Mean of each component.
o	covariances_: Covariance of each component.
o	converged_: Indicates if the EM algorithm has converged.
o	lower_bound_: Log-likelihood at the end of EM iterations.
Project Tasks
1. Estimation from Generated Data
We start with one-dimensional data to understand GMM estimation. The tasks include generating sample data, applying GMM with different numbers of components, and visualizing the results.
2. Two-Dimensional Data Estimation
The project extends to two-dimensional data, where we generate samples and estimate the GMM parameters. Visualization includes 3D plotting of the estimated density surface.
3. Model Selection with AIC and BIC
We compare the AIC and BIC criteria to choose the optimal number of components for two-dimensional data. This involves plotting normalized values of these criteria for different numbers of components.
4. Applying GMM to Real Data
We apply GMM to real-world data, such as 'textures' data, projected onto the first two principal axes using PCA. This includes constructing the GMM, verifying convergence, and visualizing the estimated density.
5. Further Analysis
We also explore the stability of the partitions using the adjusted Rand index and apply Gaussian mixture density estimation to the 'textures' data projected onto the first two discriminant axes using LDA.
