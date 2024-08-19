Epilepsy-detection-using-EEG-data

In this project, I applied machine learning models to time series data for classification purposes. My goal was to build a machine learning model that can detect epilepsy episodes from EEG time series datasets collected by Andrzejak et al. (Physical review E, 2001). 
The raw data were separated into five classes based on the souces of EEG recordings: two recordings from healthy people, two recordings from epileptic patients not having epileptic seizures, and one recording from the epileptic patients having epileptic seizures. 
In order to apply machine learnign algorithms to classify the EEG recordings, I transformed the raw data into data formats suitable for machine learning models. I first used pandas library to explore and preprocess the data, and then I transformed the data into the data format that machine learning models can accept. I applied transformation functions from cesium library to the data to produce new features that can be supplied as inputs to machine learning models. I varied the number and nature of the newly produced features to improve the accuracy of the model predictions. I separated the transformed data into training and test sets. I have built two classes of classification models: random forest classifier from scikit-learn module and gradient boosting classifier from xgboost library. I trained the models on the training sets, and later I validated the models' accuracies by generating predictions for the unseen test set and comparing them to the true class labels. The gradient boosting model outperformed the random forest model on this dataset. 
I also manipulated the number of categories in the dataset to improve the model prediction accuracy. I first developed a five-class classification model to work with  the five-categories of the recorded data. I later transformed the raw data from five categories into three categories based on insights how the data were collected: category 1: recordings on healthy people, category 2: recordings from patients when the epileptic seizures were not present, and category 3: recordings from patients with epipetic seizures. The gradient boosting classifier resulted in much higher prediction accuracy on the three-class classification problem.
Thus, in this project I showed that machine learning models can be effectively applied to time series EEG to detect epileptic seizure episodes. The raw data have been transformed into format that machine learning models can accept. I developed two classes of classifier models: random forest classifier and gradient booster classfier. The gradient booster model performed better than the random forest model, but selecting better features based on expert insights and including them into the gradient booster model resulted in the high enough classification accuracy. 
