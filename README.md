# CodeSearch-Search_Engine

## LeetCode Question Search Engine

This project is a search engine that provides LeetCode questions based on a word searched. The search engine is built using the TF-IDF algorithm and is deployed on Render.

### Steps to Build the Search Engine:

1. Scraping Question Links:
   - Used Selenium and Chrome Webdriver to scrape question links from the LeetCode website.
   - Removed duplicate links to ensure uniqueness.

2. Scraping Text from Question Links:
   - Scraped the text from each question link, excluding premium questions.

3. Storing Scraped Text:
   - Stored the scraped text in a Google Drive folder. Link: [Google Drive Folder](https://drive.google.com/drive/folders/1OdczHgBpPd_Egm_hcHLACjKP5tmL3mps?usp=sharing)

4. Data Preprocessing:
   - Preprocessed the scraped text using the `prep.py` file.
   - Cleaned and prepared the text data for further processing.

5. Generating Files:
   - `vocab.txt`: Contains the vocabulary (unique words from preprocessed text).
   - `documents.txt`: Contains the preprocessed text for each question.
   - `idf-values.txt`: Contains IDF (Inverse Document Frequency) values for words in the vocabulary.
   - `inverted-index.txt`: Contains the inverted index mapping words to documents.

6. Retrieving Search Results:
   - Utilized the generated files to retrieve search results based on user queries.
   - Results are displayed in decreasing order of the score (calculated using IDF and TF values).

### Deployed Search Engine:
The search engine is deployed on Render. You can access it at [https://query-searcher.onrender.com/](https://query-searcher.onrender.com/).


