Behavioral and Sentiment Analytics on Presidential Tweets

Project Overview
This project analyzes over 11,000 tweets from former U.S. President Donald Trump (@realDonaldTrump) to explore political communication patterns through tweet metadata, device usage behavior, and sentiment analysis. By identifying trends in tweet source, timing, and tone, the project supports claims from investigative journalism about differences in authorship and media bias.


Tools & Technologies
Languages: Python
Libraries: Pandas, NumPy, Matplotlib, re, json
Sentiment Analysis: VADER (Valence Aware Dictionary and sEntiment Reasoner)
Data Source: Twitter JSON data from  TwitterAPI @realDonaldTrump (2016–2020)

Key Objectives
1. Data Processing
Loaded JSON tweets from recent and older archives.
Normalized inconsistent text fields (text and full_text).
Merged and de-duplicated over 11,000 tweets.
Extracted structured tables with tweet IDs, timestamps, text, sources, and retweet counts.

2. Device Usage Analysis
Parsed tweet source metadata to extract device information (e.g., iPhone, Android, Web).
Discovered that iPhone was used more than 3x as often as Android.
Created hourly histograms showing that iPhone tweets were posted at different times than Android — suggesting different users or usage patterns (Trump vs. staffers).
3. Sentiment Analysis
Preprocessed tweets with regular expressions and converted to lowercase.
Joined tweet words with the VADER lexicon to assign polarity scores.
Calculated sentiment per tweet and identified:
Most positive tweets: congratulatory or national pride (e.g., World Cup)
Most negative tweets: criticisms involving political opponents or media

Compared tweet sentiment about news outlets:
Fox News tweets had a positive mean sentiment (+0.42)
New York Times tweets had a negative mean sentiment (–1.29)

📈 Visualizations
📊 Device usage bar charts
🕒 Hourly tweet histograms for Android vs. iPhone
😊😠 Sentiment distributions comparing Fox vs. NYT

✅ Key Insights
Tweet device usage reveals behavioral differences — possibly between Trump and his staff.
Peak tweet hours and device types support journalist theories about authorship.
Sentiment analysis confirms tone differences when referring to different media outlets.

Conclusion
The analysis revealed clear behavioral patterns in tweet authorship based on device and timing, aligning with journalistic hypotheses about Trump's and his staff's usage habits. Sentiment analysis further confirmed partisan tone variation, demonstrating how computational techniques can support political insight and media analysis in digital journalism.