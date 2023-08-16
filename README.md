# Car_insurance_ML

Car Insurance prediction Model

Data from kaggle: https://www.kaggle.com/datasets/ifteshanajnin/carinsuranceclaimprediction-classification

### Summary:

Data Science project that focus on predicting if a car owner with insurance is going to file a claim or not. The algoritm used was a GBR classifier. The model predicts very poorly despite the high accuracy, it is because the bad quality of the data and the class imbalance problem despite this last one was solved.

![Alt text](imagenes/Procesos.JPG)

### Steps:
First  we import the dataset from kaggle.

Then we proceed to shuffle the DS.

After that we do a Data Analysis of the Dataset in order to check for feature imabalance, class imbalance, possible predictors, skewness, outliers, kurtosis, distribution, etc.

Then we preprocess the data applying feature engineering to a few features that can be joined into one, we label encode the data, normalize the data, clipp outliers. And in order to face the CLASS IMBALANCE problem we made two runs, one was applying the Upsamle to the whole Training dataset and not applying any udnersample to the majority class, and the results were poor. On the other one we applied the Upsample to a portion of the whole Training dataset and then Undersample to another small portion of the dataset. Again the results were poor.

Next step was to apply PCA. The data had many columns that not all of them were useful and there were too many of them so maybe we could have faced the Curse of Dimensionality, so to avoid that and to get only the useful features we decided to apply a PCA.

Next step was to train the model using GBR Classifier Algorithm.

Then we use a Confussion matrix to see how good or bad the model is predicting. The accuracy is very high which really doesn't matter because it is a Class Imbalance problem. But the rest of the scores F1, Recall and Precission are very poor when predicting the minority class.

We have to remember always that the quality of the model highly depends on the quality of the data. DATA IS KING.



