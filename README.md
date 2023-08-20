# DrugCompat- Drug-excipient Compatibility Prediction Tool

DrugCompat is a powerful tool designed to predict the compatibility of drug-excipient combinations using machine learning. It is particularly useful for pharmaceutical researchers and formulation scientists who are looking to quickly assess the compatibility of various drug and excipient combinations.

Email- ganeshwaghule12@gmail.com
# Features:
1. Compatibility Prediction: DrugCompat uses a pre-trained machine learning model to predict whether a given drug and excipient are compatible or not. It analyzes the molecular fingerprints of the compounds and provides a compatibility score.

2. Advanced Graphs: The tool provides advanced graphical representations of the compatibility study results, including bar plots and pie charts, to help users visualize and interpret the results more easily.

3. Downloadable Results: Users can download the compatibility study results in PDF or DOCX formats, making it easy to share and document the findings.

4. Physical Mixture Analysis: DrugCompat automatically analyzes the compatibility of a physical mixture of all the excipients with the drug compound. This feature is particularly useful when formulating multi-component drug products.

# Installation on Google Colab:
1. Open Google Colab and create a new Python 3 notebook.
2. In the first cell, import the necessary libraries by running the following code:
```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import pubchempy as pcp
import joblib
from sklearn.tree import DecisionTreeClassifier
from sklearn.preprocessing import OneHotEncoder
from fpdf import FPDF
from docx import Document
from IPython.core.display import display, HTML
from google.colab import files
import random
```
3. Mount your Google Drive by running the following code and following the prompts:
```
from google.colab import drive
drive.mount('/content/gdrive')
```
4. Clone the DrugCompat GitHub repository to your Google Drive by running the following code:
```
!git clone https://github.com/your_username/DrugCompat.git /content/gdrive/My\ Drive/Colab\ Notebooks/drug_design/\
```
5. Load the pre-trained model and label encoder from the files in the repository by running the following code:
```
save_path = "/content/gdrive/My Drive/Colab Notebooks/drug_design/"
clf = joblib.load(save_path + 'compatibility_model.pkl')
enc = joblib.load(save_path + 'label_encoder.pkl')
```
6. Now you can use the DrugCompat tool to predict the compatibility of drug-excipient combinations, visualize the results, and download the results in PDF or DOCX formats.
# Usage:
1. Enter the name of the drug and the names of the excipients separated by commas.
2 The tool will display the compatibility results in a table format.
3. Click the "Show Graphs" button to display the advanced graphs.
4. Click the "Download PDF" or "Download DOCX" button to download the results in the desired format.
# Conclusion:
DrugCompat is a versatile and user-friendly tool that provides valuable insights into drug-excipient compatibility. It is a valuable asset for pharmaceutical researchers and formulation scientists looking to optimize drug formulations.
