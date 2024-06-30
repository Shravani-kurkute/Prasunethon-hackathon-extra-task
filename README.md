# Prasunethon-hackathon-extra-task
# Smart City Management System
## Overview
The Smart City Management System aims to enhance urban living through efficient resource management, improved public safety, and enhanced citizen engagement. This integrated system leverages web and mobile applications, machine learning algorithms, blockchain technology for security and transparency, and artificial intelligence for data analysis and decision-making.

## Project Structure
### Machine Learning Component
The machine learning component of this project involves creating predictive models to forecast city resource needs and detect anomalies in city operations. The predictive models are built using time series data and other relevant datasets.

## Data Files
1. oil.csv: Contains oil price data.
2. train.csv: Contains the training dataset with time series data.
3. test.csv: Contains the test dataset.
4. sample_submission.csv: Provides a sample submission format.
5. holidays_events.csv: Contains data on holidays and events.
6. stores.csv: Contains store-related data.
7. transactions.csv: Contains transaction data.

   ## Python Environment
   This project utilizes the Kaggle Python Docker image, which includes many helpful analytics libraries pre-installed. Some of the key packages used in this project are: 1. numpy: For linear algebra.
2. pandas: For data processing and CSV file I/O.

## Code Snippets
a) Loading Libraries:
import numpy as np
import pandas as pd

b) Reading Data:
oil_data = pd.read_csv('oil.csv')
train = pd.read_csv('train.csv', parse_dates=True, low_memory=False, index_col='date')
test = pd.read_csv('test.csv')
submission_sample = pd.read_csv('sample_submission.csv')
holidays_data = pd.read_csv('holidays_events.csv')
store_data = pd.read_csv('stores.csv')
transaction_data = pd.read_csv('transactions.csv')

c) Printing Dataset Information:
print('Number of train samples: ', train.shape)
print('Number of test samples: ', test.shape)
print('Number of store data: ', store_data.shape)
print('Number of Holiday data: ', holidays_data.shape)
print('Number of Oil Price data: ', oil_data.shape)
print('Number of features: ', len(train.columns))
print(train.info())
print(train.columns)
print(train.head())

## Custom CSS Styling
Custom CSS is applied to enhance the visual appearance of the HTML output in Jupyter notebooks. The CSS file is downloaded and read as follows:

!wget http://bit.ly/3ZLyF82 -O CSS.css -q

from IPython.core.display import HTML
with open('./CSS.css', 'r') as file:
    custom_css = file.read()

HTML(custom_css)

## HTML Content
The following HTML content is used for displaying custom styled HTML elements:
html_contents = """
<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
        <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway">
        <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto">
        <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Verdana">
        <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open Sans">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
        <style>
        .title-section{
            font-family: "Roboto", Verdana, sans-serif;
            font-weight: bold;
            color: "#6A8CAF";
            letter-spacing: 6px;
        }
        hr { border: 1px solid #E58F65 !important;
             color: #E58F65 !important;
             background: #E58F65 !important;
           }
        body {
            font-family: "Verdana", sans-serif;
            }
        </style>
    </head>
</html>
"""

HTML(html_contents)

# Usage
To run the project, load the provided datasets and execute the code snippets in a Jupyter notebook environment. The provided code snippets will help you get started with loading data, understanding the data structure, and applying custom styles to your notebook outputs.

# Contributing
Contributions are welcome! Please feel free to submit a Pull Request.



