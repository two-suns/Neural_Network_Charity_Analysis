# Neural Network Charity Analysis
## Overview
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.
## Results
* Data Preprocessing
  - The target for the model is the 'IS_SUCCESSFUL' column.
  - The feature columns include: 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', and 'SPECIAL_CONSIDERATIONS'.
  - Dropped columns inclue: 'STATUS', 'ASK_AMOUNT', 'NAME', AND 'EIN.'

* Compiling, Training, and Evaluating the Model
  -  For the initial model, there were 2 layers with 8 neurons for layer 1 and 5 for layer 2.  It used the relu activation functions for the inputs and sigmoid for the output.  This model produced 66% accuracy.
  -  Three attempts to improve the model:
    - Attempt 1: 3 layers with 10 nodes for layer 1, 7 for layer 2, and 4 for layer 3. It also used relu and sigmoid for input and output respectively.  This model produced 53% accuracy.
    - Attempt 2: Dropped back to 2 layers, but increased the neurons to 10 and 7 respectively. Again used relu and sigmoid for input and output.  This model produced 42% accuracy.
    - Attempt 3:  This attempt used 1 layer with 10 neurons.  It changed the input function to tanh and output remained the same.  This model produced 52% accuracy.

## Summary
Overall the model did not reach the threshold of 75%.  Perhaps running it again with even more neurons and dropping more columns could produce a better result.  This would give the model less to take in and more neurons to run through.
