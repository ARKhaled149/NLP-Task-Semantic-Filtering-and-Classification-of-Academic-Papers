# NLP Task: Semantic Filtering and Classification of Academic Papers

## Project Overview

This project focuses on filtering and classifying academic papers from a dataset obtained through keyword-based searches on PubMed. The primary aim is to identify papers that implement deep learning neural network-based solutions in the fields of virology and epidemiology. The dataset contains 11,450 records and is provided in CSV format.

## Objectives

1. **Semantic Filtering**: Utilize semantic natural language processing techniques to filter out papers that do not employ deep learning approaches in virology/epidemiology.
2. **Classification**: Classify relevant papers according to the type of method used: ["text mining", "computer vision", "both", "other"].
3. **Method Extraction**: Extract and report the name of the method used for each relevant paper.

## Setup and Requirements

### Prerequisites

- Python 3.x
- Google Colab (for running the notebook)
- Libraries: pandas, nltk, re, matplotlib

### Installation

To set up the environment, ensure your Google Drive is mounted in Colab to access the dataset. Install the required libraries and download necessary NLTK data files to facilitate text processing.

## Code Explanation

### Data Loading

The dataset is loaded from Google Drive using pandas. It contains abstracts of academic papers which are processed to identify relevant papers.

### Semantic Filtering

The project employs a function to filter papers that mention deep learning methods. This involves checking for keywords such as 'deep learning', 'neural network', 'CNN', 'RNN', 'LSTM', and 'transformer'.

### Classification

Papers are categorized based on the presence of 'text mining' and 'computer vision' keywords. The classification ensures that papers mentioning both methods are correctly identified.

### Method Extraction

Regular expressions are used to extract specific method names from the abstracts, helping to identify the techniques used in each paper.

### Saving Results

The processed data, including relevant papers and their classifications, is saved to a new CSV file in Google Drive.

## Usage

1. **Run the Notebook**: Execute the code in Google Colab to process the dataset.
2. **Review Results**: The output CSV file contains filtered and classified papers, along with extracted method names.

## Code Availability

The code for this project is provided in the repository as `NLP_TASK.py` and its notebook version. Both files are available for review and execution.

## Conclusion

This project effectively streamlines the early stages of article collection for review by minimizing manual scanning and filtering of numerous articles. The approach leverages lightweight NLP techniques suitable for personal computers or free platforms like Google Colab.
