# Unit 12—Tales from the Crypto

![Stock Sentiment](Images/sentimental.jpeg)

## Background

There's been a lot of hype in the news lately about cryptocurrency, so you want to take stock, so to speak, of the latest news headlines regarding Bitcoin and Ethereum to get a better feel for the current public sentiment around each coin.

In this assignment, I will apply natural language processing to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. I will also apply fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.

The following tasks will be completed:

1. [Sentiment Analysis](#1---Sentiment-Analysis)
2. [Natural Language Processing](#2---Natural-Language-Processing)
3. [Named Entity Recognition](#3---Named-Entity-Recognition)

---

### 1 - Sentiment Analysis

The [newsapi](https://newsapi.org/) was used to pull the latest news articles for Bitcoin and Ethereum and create a DataFrame of sentiment scores for each coin.

The descriptive statistics were used to answer the following questions:

1. Which coin had the highest mean positive score?
- **ANSWER: - The analysis demonstrates that Ethereum has the highest mean positive score.** 

2. Which coin had the highest negative score?
- **ANSWER: - The analysis demonstrates that Ethereum has the highest compound score.** 

3. Which coin had the highest positive score?
- **ANSWER: - The analysis demonstrates that Ethereum has the highest positive score.** 


### 2 - Natural Language Processing

In this section, I used NLTK and Python to tokenize text, find n-gram counts, and create word clouds for both coins. 

#### N-grams


1.  Use NLTK to produce the ngrams for N = 2.

    **ANSWER: - Bigrams for sample article**

    {('bitcoin', 'slumped'): 1, ('slumped', 'wednesday'): 1, ('wednesday', 'thursdayjirapong'): 1, ('thursdayjirapong', 'manustronggetty'): 1, ('manustronggetty', 'imagesbitcoin'): 1, ('imagesbitcoin', 'wa'): 1, ('wa', 'thursday'): 1, ('thursday', 'cryptocurrency'): 1, ('cryptocurrency', 'market'): 1, ('market', 'wa'): 1, ('wa', 'sea'): 1, ('sea', 'red'): 1, ('red', 'minute'): 1, ('minute', 'revealed'): 1, ('revealed', 'federa'): 1}

2. List the top 10 words for each coin.

    **ANSWER: - Top 10 words for Bitcoin**

    [('bitcoin', 88),
    ('market', 27),
    ('btc', 27),
    ('crypto', 23),
    ('wa', 22),
    ('cryptocurrency', 21),
    ('price', 16),
    ('last', 12),
    ('mining', 12),
    ('first', 11)]

    **ANSWER: - Top 10 words for Ethereum**

    [('ethereum', 35),
    ('cryptocurrency', 30),
    ('crypto', 20),
    ('eth', 19),
    ('market', 18),
    ('bitcoin', 16),
    ('wa', 15),
    ('one', 14),
    ('million', 13),
    ('blockchain', 12)]

#### Word Clouds

The following word clouds have been generated to summarize the news for each coin.

![btc-word-cloud.png](https://github.com/apfreeman/Unit-12-Tales-from-the-Crypto/blob/main/Images/btc-word-cloud.png?raw=true)

![eth-word-cloud.png](https://github.com/apfreeman/Unit-12-Tales-from-the-Crypto/blob/main/Images/eth-word-cloud.png?raw=true)


### 3 - Named Entity Recognition

In this section, I have built a named entity recognition model for both coins and visualized the tags using SpaCy.

![btc-ner.png](https://github.com/apfreeman/Unit-12-Tales-from-the-Crypto/blob/main/Images/btc-ner.png?raw=true)

![eth-ner.png](https://github.com/apfreeman/Unit-12-Tales-from-the-Crypto/blob/main/Images/eth-ner.png?raw=true)


