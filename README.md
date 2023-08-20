DrugCompat is a powerful tool designed to predict the compatibility of drug-excipient combinations using machine learning. It is particularly useful for pharmaceutical researchers and formulation scientists who are looking to quickly assess the compatibility of various drug and excipient combinations.

Features:
Compatibility Prediction: DrugCompat uses a pre-trained machine learning model to predict whether a given drug and excipient are compatible or not. It analyzes the molecular fingerprints of the compounds and provides a compatibility score.

Advanced Graphs: The tool provides advanced graphical representations of the compatibility study results, including bar plots and pie charts, to help users visualize and interpret the results more easily.

Downloadable Results: Users can download the compatibility study results in PDF or DOCX formats, making it easy to share and document the findings.

Physical Mixture Analysis: DrugCompat automatically analyzes the compatibility of a physical mixture of all the excipients with the drug compound. This feature is particularly useful when formulating multi-component drug products.

Installation on Google Colab:
1. Open Google Colab and create a new Python 3 notebook.

2. In the first cell, import the necessary libraries by running the following code:

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

Mount your Google Drive by running the following code and following the prompts:
