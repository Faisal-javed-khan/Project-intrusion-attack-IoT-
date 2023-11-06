# Project-intrusion-attack-IoT-
Ensemble-classification , using optimal attributes for the detection of various  iot Intrusion attack

<h3>Data Preparation:</h3>

The script loads CSV files from the current directory, containing labeled data for a machine learning model.
Data is split into features and labels.
Features are standardized, and labels are encoded and converted into one-hot encoded format.
Data Generator Function:

Defines a generator function called datagen that yields batches of preprocessed data.
Uses train_test_split from scikit-learn to split the data into training and testing sets.
Applies label encoding and one-hot encoding to the labels.
Yields batches of training and testing data for model training.
Data Visualization:

Utilizes Seaborn and Matplotlib to visualize the distribution of labels in the training data.
Shows a bar chart representing the count of different classes in the training data.
Neural Network Model:

Constructs a neural network model using Keras.
The model architecture includes three 1D convolutional layers followed by max-pooling layers.
Flattens the output and adds dense layers for classification.
Compiles the model using the Adam optimizer and categorical crossentropy loss.
Training Loop:

Iterates over batches of data from the generator function.
Trains the model using the training data and validates it using the testing data.
Computes precision, recall, and F1-score for model evaluation.
Displays accuracy, loss, and validation plots during training.
Model Evaluation:

Evaluates the model on the test set to calculate loss and accuracy.
Plots accuracy and loss curves to visualize the model's performance during training.
