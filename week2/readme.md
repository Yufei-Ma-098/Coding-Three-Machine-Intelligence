# Readme
>## Instruction
>Make a copy of your Coding Three notebook from Step 2.(https://git.arts.ac.uk/rfiebrink/ExploringMachineIntelligence_Spring2023/blob/main/week2/TextClassifier.ipynb)  
Find another binary (2-class) text classification dataset (e.g., from kaggle.com) and adapt the text classification week2 notebook to build a classifier for this dataset. Use your copy of the Coding Three notebook from Step 2, rather than using other code you find elsewhere. 

## Introduction
This code tries to build a fake news classifier using a neural network model implemented in Keras and TensorFlow libraries. The dataset used is "fakerealnews.csv", containing news headlines and their corresponding labels, with six different classes: 'TRUE', 'FALSE', 'barely-true', 'half-true', 'mostly-true', and 'pants-fire'. It can be found at https://www.kaggle.com/techykajal/fakereal-news.

## Prerequisites
To run this code, you will need to have the following libraries installed:
- NumPy
- TensorFlow
- Keras
- Pandas
- Scikit-learn

## Usage
1. Download or clone the repository to your local machine.
2. Open a terminal and navigate to the directory containing the downloaded files.
3. Run the following command: python fake_news_classifier.py.
4. The code will preprocess the data, build the neural network model, train the model, and evaluate its performance on the test set.
5. The test loss and accuracy will be displayed in the terminal.

## Implementation Details
1. The dataset is loaded from a CSV file using the pandas library.
2. The data is preprocessed using the TfidfVectorizer from the scikit-learn library to convert the news headlines into numerical features, and then split into training and test sets using the train_test_split function from the same library.
3. The neural network model is implemented using the Sequential class from Keras, with two dense layers: the input layer with 64 neurons, and the output layer with a single neuron and a sigmoid activation function.
4. The model is compiled with binary cross-entropy loss and Stochastic Gradient Descent optimizer with a learning rate of 0.01.
5. The model is trained for 50 epochs with a batch size of 32, and its performance is evaluated on the test set.
