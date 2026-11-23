Text Analysis Assignment – Python
1. Project Overview

This project focuses on extracting textual data from a list of URLs and performing text analysis to compute various readability and sentiment-related variables.
The complete solution is implemented using Python programming, following the structure and rules provided in the assignment instructions.

The project consists of two major parts:

Data Extraction – Scraping article title and content from given URLs.

Text Analysis – Computing sentiment and readability metrics from the extracted text.

2. Approach and Methodology
Data Extraction

The input file Input.xlsx contains URL_ID and corresponding URL.

Python libraries such as requests, BeautifulSoup, and pandas are used.

For each URL:

The article title is extracted from the <h1> tag.

The article body is extracted mainly from paragraph (<p>) tags.

Website headers, footers, navigation menus, and advertisements are excluded.

Each article is saved as a .txt file using its URL_ID as the filename.

Text Preprocessing

Before analysis, the extracted text is cleaned by:

Converting text to lowercase

Removing punctuation and extra spaces

Tokenizing text into words and sentences

Removing stopwords using NLTK

This ensures accurate and consistent text analysis.

Text Analysis

The cleaned text files are analyzed to compute the following variables:

Positive Score

Negative Score

Polarity Score

Subjectivity Score

Average Sentence Length

Percentage of Complex Words

Fog Index

Average Number of Words per Sentence

Complex Word Count

Word Count

Syllable per Word

Personal Pronouns

Average Word Length

Positive and negative sentiment scores are calculated using predefined word lists (positive-words.txt and negative-words.txt).
Readability metrics such as Fog Index and complex word percentage are calculated based on standard text analysis formulas.

3. Output

The final output is generated in Excel format (Output.xlsx).

The structure and column order strictly follow the provided Output Data Structure.xlsx.

All input variables from Input.xlsx are retained and merged with computed variables.

4. Tools and Libraries Used

Python 3.x

pandas

requests

beautifulsoup4

nltk

openpyxl

re (regular expressions)

5. Role of AI Assistance

AI tools were used only for minor guidance, such as:

Clarifying Python syntax

Understanding text analysis concepts

Verifying formulas for readability metrics

The core logic, code implementation, data handling, and problem-solving approach were developed and executed independently by me.

6. How to Run the Project

Install required dependencies:

pip install -r requirements.txt


Place Input.xlsx in the data/ folder.

Run the Python script:

python text_analysis.py


The extracted articles will be saved in:

extracted_articles/


Final output will be generated as:

Output.xlsx

7. Conclusion

This project demonstrates practical skills in:

Web scraping using Python

Text preprocessing and NLP fundamentals

Sentiment and readability analysis

Working with structured Excel inputs and outputs

The solution strictly follows the assignment guidelines and produces reproducible and accurate results.