# Automatic Text Summarization and Evaluation

## Overview:
This project implements automatic text summarization techniques and evaluation metrics using Python and various libraries such as NLTK, Gensim, NetworkX, and Rouge Score. The goal is to summarize textual documents efficiently and evaluate the quality of generated summaries against reference summaries.

## Features:
1. **Preprocessing:**
   - The text data is preprocessed to remove punctuation, tokenize sentences and words, convert words to lowercase, and remove stop words.

2. **Topic Modeling (LDA):**
   - Latent Dirichlet Allocation (LDA) is applied to identify topics within the text data. This unsupervised learning technique helps in understanding the underlying themes present in the document.

3. **Extractive Summarization (TextRank):**
   - TextRank algorithm is used for extractive summarization, where key sentences are identified and extracted from the document based on their importance. The summary is generated by concatenating these key sentences.

4. **Correction and Capitalization:**
   - The generated summary is post-processed to correct double full stops and capitalize the first letter of each sentence.

5. **ROUGE Evaluation:**
   - ROUGE (Recall-Oriented Understudy for Gisting Evaluation) scores are calculated to evaluate the quality of the generated summary against a reference summary. ROUGE measures include ROUGE-1 (unigram overlap), ROUGE-2 (bigram overlap), and ROUGE-L (longest common subsequence).

## Dependencies:
- nltk
- gensim
- sklearn
- networkx
- rouge-score

## Usage:
1. Ensure that the necessary Python libraries are installed using `pip install -r requirements.txt`.
2. Update the file paths in the code to point to the input documents and directories.
3. Run the code to perform text summarization and evaluation.

## File Structure:
- `main.py`: Main script containing the text summarization and evaluation logic.
- `utils.py`: Utility functions for preprocessing, summarization, and evaluation.
- `requirements.txt`: File containing the list of dependencies.
- `README.md`: Readme file providing an overview of the project and instructions for usage.
- `annual_reports/`: Directory containing the annual reports or documents to be summarized.
- `gold_summaries/`: Directory containing reference or gold standard summaries for evaluation.
- `generated_summaries/`: Directory where the generated summaries will be saved.
- `evaluation_results/`: Directory where the evaluation results, including ROUGE scores, will be saved.


