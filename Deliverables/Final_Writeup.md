# NLP for Digital Videogame Reviews on Amazon

## Background & Design
The videogame industry today is worth around $200 billion, and is only expected to rise in the near future. One outlet for game producers to sell their products is on Amazon, which currently has around 150 million prime subscribers, and many more regular customers. In order to increase their sales volumes and position in the industry, videogame companies need to better understand their customer base and their complaints or praises of their products.

Conducting NLP on Amazon reviews can provide companies valuable insights to the sentiments of videogame customers, and improve a products' reception, thus helping to increase sales.

## Data
The data I used for this NLP project was downloaded from [Amazon Public Datasets](https://s3.amazonaws.com/amazon-reviews-pds/readme.html). The original dataset contains 144,724 rows of review data, and 15 columns.

I mainly utilized the product_title, star_rating, and review_body columns for this project.


## Tools & Algorithms:

Data Preprocessing:
1. Removing all nonalphanumeric characters and lowercasing each review_body text.
2. NLTK's stop_word library (as well as more custom stop words)
3. Pandas for data manipulation

Vectorization:
1. Created Document-Term Matrix with TF-IDF vectorizer and CountVectorizer (TF-IDF for final)
2. Fit to LSA and NMF for topic modeling (NMF for final)
3. Sklearn for topic models
3. Interpreting and Determining 7 Topic Models

Sentiment Analysis:
1. Using provided star reviews to create a positive (4-5 stars) and negative (1-2 stars) sentiment column (Note: future work includes creating a more advanced sentiment analysis using spaCy)

Visualizations:
1. Matplotlib and Seaborn for Box Plots
2. ScatterText to create initial visualization of positive/negative review word frequencies

## Visualizations
ScatterText for Positive/Negative Words Across Entire Dataset
![scattertext](https://github.com/Jason-HKim/NLP_Project/blob/master/Visualizations/scattertest_visualization_simple_sentiment_analysis.png)
