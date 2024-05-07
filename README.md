# Scrap_BS4_Textual_Analysis

# Description of Jupyter Notebook Workflow

## Step 0: Importing Required Libraries
- Import necessary libraries for web scraping, data manipulation, and analysis including `pandas`, `requests`, `BeautifulSoup`, `os`, and `nltk`.

## Step 1: Data Extraction
- Define the `data_extraction` function to scrape text content from web pages using BeautifulSoup and save it to text files.
- Load an Excel file (`Input.xlsx`) using Pandas, containing URLs and corresponding ID columns.
- Call the `data_extraction` function for each URL in the Excel file to scrape content and save it to text files.

## Step 2: Removing Stopwords
- Load stopwords from various files and store them in a set.
- Process text files in a specified directory to remove stopwords.
- Update the text files with stopwords removed.

## Step 3: Data Analysis
1. **Calculating Scores:**
   - Calculate positive and negative scores based on lists of positive and negative words.
   - Calculate polarity score and subjectivity score using the positive and negative scores.
   - Process text files to calculate these scores, and update the results in an Excel file (`Output Data Structure.xlsx`).

2. **Calculating Metrics:**
   - Calculate various text metrics including average sentence length, percentage of complex words, syllable count, average words per sentence, total complex word count, syllables per word, personal pronouns, and average word length.
   - Calculate these metrics for each text file and update them in the same Excel file.

### Flow:
1. Data extraction is performed initially to scrape text content from web pages and save it to text files.
2. Stopwords are removed from the text files.
3. Data analysis is conducted to calculate scores and various text metrics, and the results are updated in the output Excel file.

Overall, the notebook aims to extract text data from web pages, preprocess it by removing stopwords, and conduct data analysis to derive insights and metrics from the text content.
