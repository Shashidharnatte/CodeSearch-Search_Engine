# CodeSearch-Search_Engine

• I have created a search engine that gives LeetCode questions based on word searched, this search engine works on TF-IDF algorithm
• Deployed website using render website, here is the link to the search engine: https://query-searcher.onrender.com/
• First, scrapped all question links from LeetCode websites using Selenium and Chrome Webdriver, then removed the links which are repeated
• After that scrapped the text from all the question links except premium questions from the links which I had scrapped before
• Here is the link to scrapped text: https://drive.google.com/drive/folders/1OdczHgBpPd_Egm_hcHLACjKP5tmL3mps?usp=sharing  
• Then preprocessed the data using prep.py file and obtained vocab.txt,documents.txt,idf-values.txt,inverted-index.txt files
• Files mentioned online just above are used to get results related to the searched string in decreasing order of score(idf*tf value) of the links
