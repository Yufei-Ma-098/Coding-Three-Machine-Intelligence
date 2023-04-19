# Instructions
## 1. Interactive ML with mimic
Run this mimic project to train your own pose classifier using interactive machine learning.  
Experiment, investigating the following questions:  
What sorts of mistakes does this type of classifier make most often?  
What is the most surprising thing you can get it to do right?  
How many examples do you appear to need to build an accurate classifier? Do more examples help, in general?  
## 2. Text classification with keras
Get the week2 notebooks from the Coding Three github. (Review Github resources on the main moodle page for a reminder of how to do this with Github Desktop or command line)  
Load the TextClassifier notebook in Jupyter. (Don't forget to activate your environment first, if you're using one!)  
Make sure you can run everything in the notebook. Ask for help ASAP if you get an error.  
Read the text and code carefully throughout the notebook, and ask questions about anything you don't understand.  
Complete some of the "Explore on your own" exercises at the end.  
## 3. Image classification with keras
Load the ImageClassifier notebook (from week2 in the Coding 3 github) in Jupyter. (Don't forget to activate your environment first, if you're using one!)  
Make sure you can run everything in the notebook. Ask for help ASAP if you get an error.  
Read the text and code carefully throughout the notebook, and ask questions about anything you don't understand.  
## 4. Take it further
Choose one of the following activities to take this work further:  

Extend one of the MIMIC classifier examples (e.g., this one from part 1, or this one that does object recognition) so that it does something slightly more interesting than change the colour of a square.  
Make a copy of your Coding Three notebook from Step 2. Find another binary (2-class) text classification dataset (e.g., from kaggle.com) and adapt the text classification week2 notebook to build a classifier for this dataset. Use your copy of the Coding Three notebook from Step 2, rather than using other code you find elsewhere.   
If your new dataset uses a class column that contains words (e.g., "positive"/"negative") rather than the numbers 0 and 1, use a spreadsheet such as Excel or Google Sheets to edit this column. (See Rebecca's video at FormulasInExcel.mov for a demo of how you can do this.)  
Look for the places marked "***" in the notebook for comments about how the notebook will need to change to reflect the new dataset.  
If you are comfortable coding and you feel a bit ambitious, you may choose a multi-class classification problem. Note however that you will also need to either change the encoding of the labels to a one-hot representation with a "categorical_crossentropy" loss function, or use a "sparse_categorical_crossentropy" loss function (see "Multi-Class Classification Loss Functions" section in https://machinelearningmastery.com/how-to-choose-loss-functions-when-training-deep-learning-neural-networks/ )  
