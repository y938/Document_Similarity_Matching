# Document Similarity Tool

This tool is designed to compare PDF invoices and find the most similar documents from a database of invoices. It uses text extraction, text feature extraction, and both cosine and Jaccard similarity measures to compare the documents. Additionally, it uses image similarity using ORB keypoint detection in OpenCV.

## Features

- Extract text from PDF invoices using PyMuPDF.
- Extract important features from the text such as invoice number, date, amount, and keywords.
- Calculate text similarity using TF-IDF vectors and cosine similarity.
- Calculate text similarity using Jaccard similarity.
- Calculate image similarity using ORB keypoint detection in OpenCV.
- Load a database of invoices and find the most similar invoice to a given input invoice.
- Display results in a concise manner.

## Requirements

- Python 3.x
- Required libraries:
  - `PyMuPDF`
  - `scikit-learn`
  - `numpy`
  - `opencv-python`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/y938/Document-Similarity-Matching.git
   cd document-similarity-tool
2. Install the required libraries
    ```
    pip install pymupdf opencv-python

    ```

## Usage

1. Place your training (database) PDFs in the train folder and test PDFs in the test folder.

2. Modify the database_docs and test_docs lists in the main function with the paths to your training and test PDFs.

3. Run the script

4. The script will output the most similar invoice for each test invoice along with the similarity score.


