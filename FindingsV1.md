Night 00:

1. The baseline accuracy is 83% (class 0)
2. Missing Values: cols s56,s57,59 contain 100%  missing values, and for cols s54,s55 contain 99% missing values
3. s53 columns contain incremental indexing! only 10% are duplicates!
4. There’s no duplicate observation! 
5. There’s some high correlated features presented in heatmap!

Day 01:

1. We have 20 numerical and 15 categorical columns
2. Note:
   - s12,s13,n12,n13: even though they are encoded as numeicals,(appearing as quantitative); they are actually categorical. Taking only two values
   - n3 takes discrete number in the range [0,9], not sure should I consider it categorical or not.
   - n15 takes discrete number in the range [0,6], not sure should I consider it categorical or not.
   - The distribution of numerical variables are not same, we have to normalize if no outliers are there or we have to standarize if outliers are there! consider(n1,n2,[n4:n11],n14): these 11 are truly quantitatives!
3. Outliers: There's outliers in n8,n9,n10


#### Things to DO NOW:
- Delete the features containing missing values
- convert numerical to categorical (if necessary for one hot encoding)
- handle outliers of these three columns