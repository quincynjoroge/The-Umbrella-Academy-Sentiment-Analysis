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
![Bar chart representing mentions of characters](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s1_character.png)
In the first season of "Umbrella Academy," we analyzed how the audience interacted and discussed the characters. Through this analysis, we found that Vanya was the character that generated the most conversations. With a total of 239 mentions, she clearly resonated with viewers and played a significant role in the story. Her journey from being powerless to possessing formidable abilities among her siblings was both captivating and pivotal to the plot. As she transformed from vulnerability to world-altering power, it's no surprise that she became a focal point of intense discussions and speculation. Vanya's journey solidified her status as a captivating and hotly-debated character.

Following closely behind, we found Luther with 148 mentions, and Klaus with 139 mentions. These characters captured the audience's attention and sparked discussions, indicating their importance in shaping the narrative and viewer engagement for the first season.

#### Season 2
![Bar chart representing mentions of characters](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s2_character.png)
Transitioning to Season 2, character dynamics remained a driving force behind audience discussions. Vanya, once again, took center stage with an impressive 209 mentions, a testament to her enduring impact on the storyline. 

This heightened attention to Vanya can be attributed to her unique character arc in this season. Stranded in the 1980s and grappling with amnesia, she had forgotten her extraordinary powers until her gradual recollection. Her journey of self-discovery and the looming threat of her world-altering abilities resurfacing kept viewers enthralled. In the words of Five, "Vanya is the BOMB!"—a sentiment that aptly captures the explosive intrigue surrounding her character in Season 2.

Season 2 of the show saw Diego become a more prominent character, with a total of 175 mentions. This increase in attention was due to his important role in the season's plot, as he worked tirelessly to stop the assassination of J.F. Kennedy. Additionally, his romantic relationship with the new character Lila also contributed to his popularity among viewers. Meanwhile, Klaus remained a beloved character, receiving a total of 142 mentions. His charming and magnetic personality continued to captivate audiences, making him a fan favorite that viewers couldn't get enough of.

#### Season 3
![Bar chart representing mentions of characters](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s3_character.png)
In Season 3, a notable shift occurred in the character dynamics of "Umbrella Academy." Vanya, who had previously commanded significant attention, found herself notably absent from the list of the top 5 mentioned characters. This change can be attributed to her altered character arc in Season 3, where she assumed the role of Viktor, a character that did not have a profound impact in Season 3. 

Instead, the spotlight turned to Allison, who took the lead with a substantial 633 mentions. However, this high mention count carries a distinct nuance. Unlike previous seasons, where positive character traits often fueled discussions, Allison's prominence in Season 3 was accompanied by polarizing opinions. Viewers seemed divided by the way Allison was portrayed in this season, with some perceiving her actions as selfish and potentially detrimental to her siblings. The fact that she almost sacrificed her own brothers and sisters for her personal gain seemed to provoke intense debate and criticism among the audience. 

This shift in character dynamics and audience perceptions in Season 3 highlights the series' ability to evolve and challenge viewers' expectations, offering a different dimension to character interactions and storytelling. It also shows the complex and multi-dimensional nature of character development, where characters can be both central and polarizing in the narrative.
## Sentiment Analysis
This report presents the findings of sentiment analysis conducted on the comments and discussions for each season of "Umbrella Academy" using two different sentiment analysis tools: TextBlob and VADER. The analysis aimed to understand the overall sentiment of audience reactions and identify any trends or changes in sentiment across the seasons.

### Season 1 Sentiment Analysis
#### TextBlob:
**Positive Sentiment: 60.1% | Negative Sentiment: 25.9% | Neutral Sentiment: 13.9%**
![Bar chart representing sentiment analysis](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s1_textblob.png)

#### VADER:
**Positive Sentiment: 54.9% | Negative Sentiment: 34.9% | Neutral Sentiment: 10.2%**
![Bar chart representing sentiment analysis](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s1_vader.png)

### Season 2 Sentiment Analysis
#### TextBlob:
**Positive Sentiment: 54.6% | Negative Sentiment: 23.7% | Neutral Sentiment: 21.7%**
![Bar chart representing sentiment analysis](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s2_textblob.png)

#### VADER:
**Positive Sentiment: 55.4% | Negative Sentiment: 29.2% | Neutral Sentiment: 15.3%**
![Bar chart representing sentiment analysis](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s2_vader.png)

### Season 3 Sentiment Analysis
#### TextBlob:
**Positive Sentiment: 53.3% | Negative Sentiment: 29.7% | Neutral Sentiment: 17.0%**
![Bar chart representing sentiment analysis](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s3_textblob.png)

#### VADER:
**Positive Sentiment: 47.7% | Negative Sentiment: 39.9% | Neutral Sentiment: 12.4%**
![Bar chart representing sentiment analysis](https://github.com/quincynjoroge/The-Umbrella-Academy-Sentiment-Analysis/blob/main/s3_vader.png)

### Sentiment Analysis Trends
#### Positive Sentiment:
Across all three seasons, positive sentiment was consistently the most prevalent sentiment. However, there is a slight decline in positive sentiment from Season 1 to Season 3 according to both TextBlob and VADER. This decline suggests that while positive sentiment remained dominant, it may have become slightly less pronounced over time.

#### Negative Sentiment:
Negative sentiment, as measured by both TextBlob and VADER, increased from Season 1 to Season 3. Season 1 had the lowest negative sentiment, while Season 3 had the highest negative sentiment. This suggests a growing presence of negative opinions or criticisms as the series progressed.

#### Neutral Sentiment:
Neutral sentiment remained relatively stable across the seasons, with only slight fluctuations. While it's the least dominant sentiment category, it did not exhibit significant changes over the course of the series.

## Conclusion
The sentiment analysis of "Umbrella Academy" comments and discussions revealed some interesting trends. While positive sentiment remained the most prevalent, there was a decline in its prominence and an increase in negative sentiment from Season 1 to Season 3. This suggests that as the series developed, it may have elicited more mixed or critical reactions from the audience. These findings could be indicative of the evolving nature of the show's content, character arcs, or plotlines. Further qualitative analysis of the comments and discussions from each season may provide deeper insights into the reasons behind these sentiment shifts.





