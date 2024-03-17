# Intro NLP - Final Project: Booking Attractions Reviews - Sentiment Analysis

## We Scraping on Booking attraction sections, from 2022 March to 2024 March
 ### Method:
 ### 1. Scraping
 #### We scraped for 4 similar cities but different in 2 high, low seasonal cities, 2 popular, non-popular cities
 ##### Seasonal:   High          Low; (Popular is based on number of reviews)
 ##### Popular Yes Barcelona     Paris
 ##### Popular Non Venice        Florance
 #### Selenium + Beautiful Soup: for human-like scraping, and local htlm elements extraction. 
 #### Regex: for text preprocessing of each html elements.text

 ### 2. DataCleaning & DataPreprocessing
 #### clean data, translate to english
 #### tokenizer + tf-idf, analysis on tf-idf

 ### 3. Sentiment Analysis
 #### Sentiment Analysis on reviews, average by months of that year

 ### 4. Dimensionality Reduction
 #### After Reduction, Analysis on the group/topics appeared

 ### 5. Diff-in-Diff
 #### Diff-in-Diff, treatment = high,low seasonal.
