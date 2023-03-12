# Natality_final
Infant Mortality 

This jupyter notebook explores the viability of using various types of classifiers to predict the survival of an infant based on data available from the birth certificate. The data is from https://www.nber.org/research/data/linked-birthinfant-death-cohort-data for the year 2015. 

A subset of this data was created by selecting particular columns. This subset was then cleaned and prepared for classification. One of the primary difficulties of using this data is that it is very unbalanced as the infant mortality rate in the united states is relatively low. While there were just under four million births in 2015 there were barely more than twenty-three thousand infant deaths. To deal with this imbalance, a random undersampling tool was used in order to create a balanced data set consisting of just forty-six thousand rows. 

Of all the classification methods that were applied to this problem the maximum accuracy that could be obtained was 82% (for a balanced test set). A significant portion of the predictive power of every classifier boiled down to one feature, namely the 5-minute APGAR score. This is unsurprising as the APGAR score is a metric for the well-being of an infant 5 minutes after it is born. 

A potentially interesting alternative to predicting the mortality of an infant would be to predict the 5-minute APGAR score itself using only features that would be available to a medical professional previous to birth. However, This task would share many of the same pitfalls with the prediction of mortality: the vast majority of infants are born relatively healthy, and as such the data is extremely imbalanced

