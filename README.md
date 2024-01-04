# SMS_SpamText_Classifier

Summary:

This project uses TfidfVectorizer from scikit-learn to convert text messages into numerical vectors (TF-IDF representation), and it uses LabelEncoder to convert categorical labels 
('ham' and 'spam') into a numeric format for data preprocessing.
The neural network architecture involves dense layers with various activation functions and a final layer using a sigmoid activation function, 
ideal for binary classification (distinguishing between spam and non-spam).
It then compiles the model with the Adam optimizer and binary cross-entropy loss function, and trains the model on the training data for five epochs, 
using a batch size of 32.
Finally, I define a predict_message function, to predict whether a new message is spam or not. It employs the previously established TF-IDF Vectorizer to convert the new message into a numerical vector. 
The trained neural network then predicts the message's classification, considering a threshold of 0.5; messages below this are labeled as 'ham,' 
while those above are labeled as 'spam'.

Instructions for this project can be found at:
  https://www.freecodecamp.org/learn/machine-learning-with-python/machine-learning-with-python-projects/neural-network-sms-text-classifier
