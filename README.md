# Intro NLP - Final Project: Booking Attractions Reviews - Sentiment Analysis

## We Scraping on Booking attraction sections, from 2021 Jan to 2024 March
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
 #### find reviews relation with months, rating - we descard to impute not-commented reviews with KNN imputing by Rating and Months.
 ##### Rating(conatins too many variance with sentiment score)
 #### after looking months relation and review numbers, we pick 2023 Jan to 2024 Jan.

 
 ### 3. Sentiment Analysis
 #### Sentiment Analysis on reviews, average by months of that year, imputing not-commented reviews with average sentiment score of that month and city
 #### after looking months relation and Sentiment score, we pick 2023 Jan to 2024 Jan.

 ### 4. Diff-in-Diff
 #### Diff-in-Diff, treatment = high,low seasonal.
 #### tokenizer + tf-idf, analysis on tf-idf


 ### 5. Dimensionality Reduction ---- not implemented yet:
 #### After Reduction, Analysis on the group/topics appeared
