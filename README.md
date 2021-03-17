# Genetic-models
implementation algorithms on genetic dataset
about the dataset : 36=n of sampling that are composed from 1000=m sites , 1..,17 samples are from Colon tissue, and 18,..,36 samples are from Lung tissue.
Our goal is to identify sites with different Methylation between the types of tissue.
Steps : First implementation of statistical test (hypothesis, pvalues and ect.), Second try to find pattern of the pvalues and ect, Third implementation of algorithms: 
1) The Westfall and Young permutation is to compute the p-value estimation: 1) P-values are calculated for each gene based on the original data set. 2) The permutation method creates a some data set by dividing the 3) P-values for all genes are computed on the some data set. 4)the min new p-values are retained and compared to the original ones. 5) This process is repeated a large number of times, and the proportion of resampled data sets where the minimum of the p-value for the new genrete data is less than the original p-value is the the correct p-value
2) Holm's procedure; Holm-Bonferroni method; Sequentially rejective Bonferroni test - sort the vector of pvalue in ascending order, we want to take_min_purn the index of the bound we need to check the index if the  pvalue is the rejection index we stop and take_min_purn the index of the pvalue  the h0 we continue.
3) benjamini hochberg procedure (BH) : For a desired false discovery rate threshold q, first of all in BH diffcedure we need to sort the vector of pvalue in ascending order generted form n hypotesis tests, We need to find the biggest index that for him we will reject all the hypotesis until that point that we find is the max of tejection, reduce the index if the term happen,Stop and take_min_purn the the index that get the bound.

Fourth : Estimate models on bootstrapped data
Bootstrapping is a highly flexible re-sampling procedure that can be used to estimate the sampling distribution of any statistic
Fifth: value the models

Sixth: Select the 5 smallest pvalue of the sites and build CI, false coverage rate (FCR) is the average rate of false coverage. not covering the true parameters, among the selected intervals.

for getting taste (image): 

<img width="482" alt="results of bootstrapping on the algorithms" src="https://user-images.githubusercontent.com/57616193/111460368-939c5280-8724-11eb-874b-58daf6db22c7.png">

