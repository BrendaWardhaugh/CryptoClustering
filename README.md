# CryptoClustering

Python and unsupervised learning are used to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

### Preparing the Data
Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.
Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

### Find the Best Value for k Using the Original Scaled DataFrame
ploting the elbow curve

![k value elbow](https://github.com/BrendaWardhaugh/CryptoClustering/assets/120147552/e76dc430-d3dc-47e0-b641-a96577072ad8)

### Cluster Cryptocurrencies with K-means Using the Original Scaled Data

![scatter 1](https://github.com/BrendaWardhaugh/CryptoClustering/assets/120147552/ca4f9fd8-a930-4249-8f76-272b3cdab501)

### Optimize Clusters with Principal Component Analysis
What is the total explained variance of the three principal components?
89.5%

![variance](https://github.com/BrendaWardhaugh/CryptoClustering/assets/120147552/316a0cc0-4110-4ee8-81f5-e5f53350a2dc)

![image](https://github.com/BrendaWardhaugh/CryptoClustering/assets/120147552/4cefaf6a-e974-4f3b-a829-1eeaddde62c7)

### Find the Best Value for k Using the PCA Data
What is the best value for k when using the PCA data? The best value for K is 4.
Does it differ from the best k value found using the original data? There is no difference in K values before or after applying PCA.

![image](https://github.com/BrendaWardhaugh/CryptoClustering/assets/120147552/5420c7dc-97cf-42fb-a843-207979d0723d)

### Cluster Cryptocurrencies with K-means Using the PCA Data

![image](https://github.com/BrendaWardhaugh/CryptoClustering/assets/120147552/14137acf-80bb-4ae3-b4a6-463d70fe1bc0)

What is the impact of using fewer features to cluster the data using K-Means? The K values did not change even after applying PCA. The clustering is more clean using PCA compared to the oringinal data.
