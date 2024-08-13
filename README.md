# 📰 TextInsight Pro

This project provides a comprehensive solution for extracting and analyzing text data from web articles. It combines various techniques for text extraction, sentiment analysis, and readability evaluation, making it a powerful tool for data scientists and researchers.

## Overview

The tool automates the extraction of article content from provided URLs, processes the text using stop words and sentiment dictionaries, and performs in-depth text analysis to generate various readability and sentiment metrics. The results are saved in CSV format for further analysis and review.

## Features

- **Text Extraction:** Extracts article content from web pages, handling cases where content is not available.
- **Sentiment Analysis:** Analyzes text to determine positive and negative sentiment scores.
- **Readability Metrics:** Calculates various readability indices and text complexity metrics.
- **Modular Functions:** Provides reusable functions for text cleaning and analysis.

## Libraries Used

- **Pandas:** For reading and processing data from Excel files and saving results to CSV.
- **Requests:** For making HTTP requests to fetch web page content.
- **BeautifulSoup:** For parsing HTML and extracting article text.
- **NLTK:** For natural language processing tasks, including tokenization and stop word removal.
- **OS:** For file and directory management.

## Functions Created

- **`extract_article_text(url)`**: Extracts article text from a given URL using BeautifulSoup. Handles errors and cases where content is not found.
- **`clean_text(text)`**: Cleans and tokenizes text, removing stop words and non-alphanumeric characters.
- **`text_analysis(article_text)`**: Analyzes the cleaned text to compute sentiment scores, readability metrics, and text complexity. Returns a dictionary of results including:
  - Positive Score
  - Negative Score
  - Polarity Score
  - Subjectivity Score
  - Average Sentence Length
  - Percentage of Complex Words
  - Fog Index
  - Average Number of Words Per Sentence
  - Complex Word Count
  - Word Count
  - Syllable Count Per Word
  - Personal Pronouns
  - Average Word Length

## Usage

1. **Prepare Your Data:**
   - Upload your Excel file containing URLs to extract text from.
   - Place stop words and sentiment dictionary files in the appropriate directories.

2. **Run the Script:**
   - Execute the provided script to perform text extraction and analysis. Results will be saved in the specified output directory.

3. **Analyze Results:**
   - Review the generated CSV files for detailed text analysis results.

## Installation

Clone the repository and install the required libraries:

```bash
git clone https://github.com/yourusername/your-repository.git
cd your-repository
pip install -r requirements.txt
