# PCA


You are asked to implement PCA (Principle Components Analysis) algorithm, project the high-dimensional data to 2 dimensions, and plot the 2-dimensional data points. 

Dataset Description: 
You are expected to conduct dimensionality reduction on three biomedical data files (pca_a.txt, pca_b.txt, pca_c.txt), which can be found on Piazza. 
In each file, each row represents the record of a patient/sample; the last column is the disease name, and the remaining columns are features. Note that your code should be able to handle the data with different numbers of rows/columns. 

Required Tasks: Please take the following steps: 
STEP 1: 
You can use your preferred programming language(s). You need to implement the PCA algorithm by yourself. Applying existing package(s) to conduct PCA directly will not receive any credit. If you are not sure about whether it is OK to use a certain function, please post your question on Piazza. 
STEP 2:
Implement PCA and then run it on three data files (pca_a.txt, pca_b.txt, pca_c.txt) to get the two-dimensional data points. For each dataset, draw the data points with a scatter plot, and color them according to their disease names. Make sure your plots are readable and colors are distinguishable. 
STEP 3: 
Apply existing packages to run SVD and t-SNE algorithms (you do NOT need to implement them by yourself) and get the two-dimensional data points. Visualize the data points of the two algorithms on the three datasets in the same way as the visualization of PCA results in STEP 2. 


##Solution

How PCA Works ?

![pca_read_me](https://user-images.githubusercontent.com/71369489/193938638-814ec11a-8903-48aa-b3f5-6be84f481b57.png)

Step1: Find the mean and SD for the data set features not considering the target variable. 

Step2: Calculate the covariance of the dataset features.

Step3: FInd the eigen vectors and eigen values for the dataset.

Step4: obtain the essential or number of features from the vectors according to the req of your n_components value.

#Execution:

--> Run the PCA.py file  : 
     <img width="241" alt="Screen Shot 2022-10-04 at 3 21 53 PM" src="https://user-images.githubusercontent.com/71369489/193940939-67498c0a-51f2-43dc-aa88-168a970a3d3e.png">

    --> The first input is the file path of the data set. So provide the path of the csv file
    --> The second input is the number of components.
    
    After providing the details: the new dataframe with n_components columns are generated. You can also get the 2-d graph according to the target column.
  
