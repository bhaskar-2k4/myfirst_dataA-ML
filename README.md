IRIS FLOWER CLASSIFICATION USING LOGISTIC REGRESSION (WITH DATA VISUALIZATION)

This project provides a clear, step-by-step demonstration of how to analyze the Iris Flower Dataset, visualize its patterns, and build a Logistic Regression model to classify iris species.
It is designed to help beginners understand how data flows from loading → visualization → modeling → prediction.

📂 Dataset Information

Source: Kaggle

Total Rows: 150

Total Columns: 6

Dataset Columns

Id

SepalLengthCm

SepalWidthCm

PetalLengthCm

PetalWidthCm

Species

The dataset must be saved as:

iris.csv


Place it in the same folder as your Jupyter Notebook.

🪜 Steps Performed in the Notebook
1. Importing Required Libraries

The notebook uses:

pandas → for loading & handling data

matplotlib.pyplot → for graphs & visualizations

LogisticRegression (sklearn) → for building the classification model

2. Loading the Dataset
iris_data = pd.read_csv("iris.csv")


This loads the Kaggle dataset into a Pandas DataFrame.

3. Viewing the Dataset

To quickly understand the data:

iris_data.head() → shows the first 5 rows

iris_data.tail() → shows the last 5 rows

These help verify the dataset is correct and properly loaded.

4. Dataset Summary

iris_data.info() → displays column types, non-null counts

iris_data.describe() → provides statistical summary (mean, min, max, std, etc.)

This confirms there are no missing values and shows how each feature behaves.

📊 Data Visualization (Matplotlib)

Visualizing the dataset helps understand species differences and feature patterns.

A) Scatter Plots

Used to show relationships between features for each iris species:

Sepal Length vs Sepal Width

Petal Length vs Petal Width

Each species is plotted separately using a loop.
These scatter plots clearly show how species form distinct clusters.

B) Histograms

Histograms were plotted for all measurement columns:

SepalLengthCm

SepalWidthCm

PetalLengthCm

PetalWidthCm

These help understand:

The distribution of values

Common vs rare ranges

Variation in measurements

C) Boxplots

Boxplots help identify:

Medians

Quartiles

Spread of the data

Outliers (if any)

A combined boxplot for all numeric columns was displayed.

🧪 Preparing Data for Logistic Regression
Feature Matrix (X):
['SepalLengthCm', 'SepalWidthCm', 'PetalLengthCm', 'PetalWidthCm']

Target Variable (y):
['Species']


These columns are used to train the model to predict the flower species.

🤖 Building the Logistic Regression Model

The model is created and trained using:

model = LogisticRegression(max_iter=200)
model.fit(X, y)


Here, the model learns directly from the entire dataset.

🔮 Making Predictions

The notebook demonstrates:

Predicting species for the entire dataset (model.predict(X))

Predicting species for a custom input sample created using a DataFrame

This shows how to use the trained model for classification.

🛠 Requirements

The project uses the following Python libraries:

pandas

numpy

matplotlib

scikit-learn

Install everything using:

pip install -r requirements.txt

🚀 How to Run the Project

Download:

Notebook file

iris.csv dataset

requirements.txt

Install dependencies

Open Jupyter Notebook

Run all cells in order

👤 Author

Name: Bhaskar
Dataset: Kaggle – Iris Flower Dataset
Project: Iris Flower Classification with Visualization using Logistic Regression