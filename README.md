# Machine_Learning_Project_of_Hotel_Booking_Demand

This preject is using ML to predict a guest will actually come or not.

Data collect from science direct.com and kaggle.com

Compare the accuracy score of all models before and after hyper tuning. We can see that Logistics regression, AdaBoost and XGB Classifier have greatest improvement in accuracy scores after hyper tuning. But overall, XGB and Random Forest have highest accuracy scores, which are around 89%.

I also did a ROC analysis on different models. Here, we can also see the plots for XGB and Random Forest are higher than the rest of the ROC curves, which indicate that they are best for classifying the dataset correctly. On the other hand, the pink curve for logistic regression is closest to the centre and performs the worst.

After finishing the models, I used the SKLearn in-built feature importances to get the weights of the features. For random forest, there are around 10 features that have particularly high weights. On the other hand, for XGB classifier, there is a feature with disproportionately high weight, which is a no refund deposit type and it has a weight of 0.847. 

Without hyper tuning, we can see that random forest now have an accuracy of 87% while XGB has 81%. We can see that although we are only using 10 of the 50 features, the accuracy is still relatively high, showing that using only the features with high weight can allow us to train models more efficiently and without the cost of getting too much information while at the same time retaining a high enough accuracy scores.

In summary, it seems that for dataset, permutation importance is more suitable for XGB classifier, while SKLearn in-built feature importance is better with Random Forest. From the analysis, we can also derive some important features that hotels can consider, including country of origin, lead time, deposit type, previous cancellations, total number of special requests, and required number of parking spaces.
