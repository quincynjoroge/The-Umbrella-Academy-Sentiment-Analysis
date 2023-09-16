# The Umbrella Academy Sentiment Analysis
![Image of the Umbrella Academy Main Cast ie. Number 1 to Number 7](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/brelly.png)

## Project Scope and Objectives:
Comparing sentiment across the three seasons and identifying the most talked-about character.
### Specific research questions:
1. How does the sentiment vary across episodes and seasons?
2. Which characters are most frequently mentioned or discussed in user-generated content per season?
## Data Collection
### Reddit
To collect data from Reddit, the Python Reddit API Wrapper (PRAW) was utilized. Data was gathered from two main Reddit groups related to "Umbrella Academy":

r/UmbrellaAcademy: This subreddit contains general discussions, fan theories, and news related to the series.
r/TheUmbrellaAcademy: This subreddit is specifically focused on discussions about "The Umbrella Academy" series.
#### Season-specific Data
To ensure relevance to each season, data was collected from threads that were specific to individual seasons. This approach allows for a more in-depth analysis of each season's reception and discussions.
### YouTube
YouTube comments related to "Umbrella Academy" were collected by visiting videos posted by movie reviewers and content creators who discussed the series. These comments provide insights into the audience's opinions and reactions to various aspects of the show.

## Preprocessing
In this section, we will discuss the data preprocessing steps performed on the combined dataset of YouTube comments and Reddit comments specific to each season of "Umbrella Academy."
These preprocessing steps ensure that the data is consistent, clean of noise, and ready for Sentiment Analysis.

### Combining YouTube and Reddit Data
Before preprocessing, we combined the datasets for each season. This merging process allowed us to consolidate comments from two distinct sources into one cohesive dataset, facilitating subsequent analysis.

### Handling Missing Values
We observed missing values in the YouTube comments dataset for Season 3. To ensure data quality and consistency, we chose to remove rows with missing values from this dataset. This step was essential to prevent potential inaccuracies in the analysis.

### Text Data Cleaning Function
A custom text data cleaning function was defined to prepare the text data for analysis. This function performed the following preprocessing steps:

**Lowercasing Text**: Text was converted to lowercase to ensure uniformity and to avoid case-sensitive issues.

**Expanding Contractions**: Contractions such as "don't" were expanded to their full forms (e.g., "do not").

**Removing Numbers**: Numeric characters were removed from the text as they often do not contribute meaningfully to textual analysis.

**Removing Punctuation**: Special characters and punctuation marks were removed to focus on textual content.

**Tokenization**: Text was tokenized into individual words. This step is essential for further analysis as it breaks down sentences into manageable units.

**Removing Stopwords**: Common stopwords (e.g., "the," "and," "is") were removed from the text as they typically do not carry significant meaning.

**Lemmatization**: Each word was lemmatized, reducing inflected words to their base or dictionary form. This helps in standardizing words (e.g., "running" becomes "run") for analysis.

**Converting Emojis to Words**: Emojis were converted to their corresponding textual representations to incorporate them into the text analysis.

## Character Analysis
To identify the characters mentioned in the text data, we implemented a character extraction process. Based on the frequency counts, we identified the characters who were the most talked about in each season. These characters had the highest number of mentions or discussions associated with them, indicating their prominence in audience conversations.
### Results
The character analysis yielded insights into the most talked about characters for each season of "Umbrella Academy.
#### Season 1 

## Sentiment Analysis

