# Sentence Similarity Calculation using Sentence-BERT

This repository contains code to calculate the similarity between sentences using Sentence-BERT, a variant of the BERT model fine-tuned for sentence embeddings.

## Overview

- **Model:** We utilize the pre-trained Sentence-BERT model 'paraphrase-MiniLM-L6-v2' from the Sentence Transformers library. This model generates high-quality sentence embeddings, enabling us to calculate the similarity between pairs of sentences.
- **Data Preparation:** We read data from two different sheets in an Excel file, assuming each sheet contains columns named 'Sentence1' and 'Sentence2'. Adjustments can be made based on actual column names in the Excel sheets.
- **Similarity Calculation:** We calculate the similarity scores between corresponding pairs of sentences from 'Sheet1' and 'Sheet2'. The similarity is computed using cosine similarity between the sentence embeddings obtained from the Sentence-BERT model.
- **Results:** The similarity scores are added as a new column ('Similarity_Score') to one of the DataFrames (assuming they have the same length). The results are then saved back to an Excel file.

## Instructions

### Prerequisites

- Install Python (3.x recommended) and the necessary libraries: pandas, sentence-transformers.

### Usage

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/sentence-similarity-calculator.git
    ```

2. Navigate to the project directory:

    ```bash
    cd sentence-similarity-calculator
    ```

3. Run the Python script `calculate_similarity.py`:

    ```bash
    python calculate_similarity.py
    ```

4. Ensure that the Excel file 'Book1.xlsx' contains two sheets named 'Sheet1' and 'Sheet2' with columns 'Sentence1' and 'Sentence2'. Adjust the column names if necessary.

5. The script will calculate similarity scores between corresponding pairs of sentences from 'Sheet1' and 'Sheet2', add the scores to 'Sheet1', and save the results to a new Excel file named 'output_file.xlsx'.

## Acknowledgments

- The code in this repository is for educational purposes and may require further customization for real-world applications.
- Feel free to modify and extend the code according to your specific requirements.

