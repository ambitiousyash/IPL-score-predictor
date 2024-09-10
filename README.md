# IPL-score-predictor

AIM:Since it is difficult for humans to find patterns in such large amounts of data, deep learning and machine learning are used to predict IPL scores. These cutting-edge methods use historical performance data from teams and players to build models for more accurate outcome prediction. IPL Score In live prediction benefits immensely from deep learning models that take into account multiple factors to produce more accurate outcomes, whilst typical machine learning methods only offer middling accuracy.

DESCRIPTION:
1)Pre-processing of Data: 
  Eliminating Superfluous Features:
  Several columns from the original DataFrame have been removed to produce a new dataframe.
  The remaining columns in the new DataFrame are where  I will train the predictive model.

2)Additional Pre-Processing:
  The data frame has been divided into independent (X) and dependent variables (y). Our final variable of interest is the overall score. 

3)Encoding of Labels:
  Label encoding has been applied to category features in X.
  For every categorical feature, I  made a different LabelEncoder object and encoded its data.
  To aid in the interpretation of the outcomes, I have developed mappings that restore the original values of the encoded labels.  

4)Train Test Divided
  The data has been divided into testing and training sets. Thirty percent of the dataset is in the test set, while the remaining seventy 
  percent is in the training set.
  The training data for input features are located in X_train.
  The testing data for input features are contained in X_test.
  The training data for target variable is located in y_train.
  The testing data for target variable can be found in y_test.

5)Scaling Features
  To make sure all of the features in our input are scaled equally, I ran our features via Min-Max scaling.
  In order to enhance model performance, scaling is done to guarantee consistent scale.
  Using the scaling parameters, scaling has changed the training and testing data.

6)Explain what a neural network is.
  TensorFlow and Keras have been used to define a neural network for regression.
  Because the regression is resilient against outliers, I have constructed the model using the Huber Loss after it has been defined.

7)Using the scaled training data, I have trained the neural network model.

8)Model Assessment
  Using the testing data, I have made predictions using the trained neural network.
  Based on the learnt patterns by the model, the variable predictions holds the estimated total run scores for the test set.

9)How about we make an interactive widget?
  Using ipywidgets, I have developed an interactive widget that uses user input for venue, batting team, bowling team, striker, and bowler 
  to estimate the score.
  To choose values for the location, batting team, bowling team, striker, and bowler, I have developed dropdown widgets.
  Next, a "Predicted Score" button widget has been added. The predict_score function will be triggered if the button is clicked, and it will 
  then carry out the subsequent actions:
  returns the user-selected values to their initial category values by decoding them.
  Scales and encrypts these variables to conform to the model training format.
  makes a prediction based on user input using the trained model.
  shows the anticipated score.

LIBRARIES:
  NumPy
  Pandas
  Scikit-learn
  Matplotlib
  Keras
  Seaborn

TECHNOLOGY USED:Machine Learning,Deep Learning,TensorFlow.  
