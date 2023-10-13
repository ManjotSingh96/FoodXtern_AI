# FoodX_AI

This project aims to predict what a student will order based on their information (Year of Study, Major, University) using a RandomForestClassifier model.

## Data
The data is loaded from a Google Sheet into a pandas DataFrame. It includes information about the students (Year of Study, Major, University) and what they ordered.

## Data Preparation
The ‘Order’ column, which is the target variable, is separated from the rest of the data. The categorical variables in the data are then encoded into numerical values using an OrdinalEncoder. The data is split into training and testing sets.

## Model
The RandomForestClassifier from sklearn is used as the predictive model. This model is an ensemble learning method that operates by constructing multiple decision trees and outputting the class that is the mode of the classes of the individual trees.

## Training
The model is trained on the training set using the fit method of the RandomForestClassifier.

## Testing
The performance of the model is evaluated on the testing set. A classification report is printed to show key metrics like precision, recall, and F1-score.

## Pickling
The trained model, along with the scaler and encoder used in data preparation, are pickled for future use.

## Prediction Function
A function is provided that takes in a user’s information (Year of Study, Major, University) and returns a prediction of what they will order. It does this by preparing the input data in the same way as your training data, and then calling the .predict() method on your trained model.

To run this project, follow the steps below:

### 1. Install Necessary Libraries
Make sure that the necessary libraries (gspread, pandas, sklearn, matplotlib, seaborn, and pickle) are installed in your Python environment. You can install these using pip:

```bash
pip install gspread pandas sklearn matplotlib seaborn pickle5
```
### 2. Clone the GitHub Repository
Clone the GitHub repository containing the code to your local machine

### 3. Run Jupyter Notebook
Navigate to the directory containing the code and start Jupyter Notebook:

```bash
cd path_to_code
jupyter notebook
```
### 4. Open the Notebook
In the Jupyter Notebook interface in your web browser, click on the predict.ipynb or predictGraph.ipynb to open it.

### 5. Run the Code
Click on each cell in the notebook and press Shift + Enter to run the code. Make sure to run the cells in order.

### 6. Enter Student Information
When prompted, enter information about a student (Year of Study, Major, University) to get a prediction of what they will order.
