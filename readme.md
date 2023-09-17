# Informal Analysis of Twitter Usage Amidst the COVID-19 Pandemic

## Overview
In this project, we have analyzed a dataset of tweets related to the COVID-19 pandemic to gain insights into how people are using Twitter to express their emotions and opinions during this challenging time.

## Data Source
The data, which includes a sample of 1000 tweets with COVID-19-related hashtags like #COVID19, #corona was gathered using the Twitter API. After the data had been cleaned up of stopwords, punctuation, and URLs, it was subjected to several natural language processing techniques for analysis.

## Using LDA for Topic Modeling
Topic modeling using LDA, an unsupervised machine learning method that separates topics from a collection of documents, was the first step. Tokenizing, lemmatizing, and stopword elimination were done during the preprocessing of the tweets. The most crucial subjects in the tweets were then determined using the LDA model, which had been trained on the preprocessed data. Coherence ratings were used to estimate the ideal amount of topics. To give an overview of each topic, the top words for each topic were printed.

## Sentiment Analysis
The dataset we have generated in this project is a CSV file containing tweets related to COVID-19 and is saved in `tweet_sentiments.csv`. The dataset includes the following columns:

- `Tweet`: The tweet's content.
- `Extremity`: A numeric score demonstrating the feeling extremity of the tweet (going from -1 to 1, where -1 is extremely pessimistic and 1 is exceptionally good).
- `Personality`: a numerical score ranging from 0 to 1, where 0 is very objective and 1 is very subjective, indicating the tweet's subjectivity.

In order to classify the tweets into positive, neutral, and negative groups based on their polarity ratings, we first performed sentiment analysis on them. We found that out of 500 tweets, 196 tweets were positive, 184 were neutral, and 120 were negative. (These values differ every time we run the code)

## Emotion Analysis
We then performed emotion analysis on the tweets using the VADER sentiment analyzer and a set of predefined emotion categories (fear, happiness, sorrow, and neutral). We first identified the dominant emotion category for each tweet based on the presence of specific keywords in the tweet. If no emotion category was identified, we used the VADER sentiment scores to determine the dominant emotion category.

The results of the emotion analysis showed that out of 500 tweets, 43.6% expressed happiness, 31.6% expressed sorrow, 20.2% expressed fear, and 4.6% were neutral. (These values differ every time we run the code)

## How to Run the Code
1. Install Jupyter Notebook and Python 3.9 on your computer.
2. Download the repository from Blackboard in .zip format, extract it, and open the folder in Visual Studio Code.
3. Run the file using the run code.
4. Visual Studio Code should now display the project folder.
5. By hitting Ctrl + Shift + in VSCode, the terminal will be displayed.
6. In the terminal, type `jupyter notebook` and hit Enter. Alternatively, run directly using the run icon.
7. Find the `index.ipynb` file by navigating to it in the Jupyter Notebook browser window.
8. Use the Run button or the keyboard shortcut Shift + Enter to run each cell in turn after opening the `index.ipynb` file.
   
Note: Before running the code, be sure to install the external libraries that the `index.ipynb` file utilizes. Do note that the results would be different each time you run the code.

## Research Paper
For more detailed information about our analysis and findings, you can read our research paper [here](https://github.com/aasthas2022/Informal-Analysis-of-Twitter-Usage-Amidst-the-COVID-19-Pandemic/blob/main/Research%20Paper%20PDF.pdf).


## Conclusion
Our analysis provides insight into how people are using Twitter to express their emotions and opinions during the COVID-19 pandemic. The majority of tweets, on the whole, showed happiness, but a sizeable number also included expressions of sadness and dread. These findings can help in understanding how the epidemic affects people emotionally and in creating therapies to help people through these trying times.
