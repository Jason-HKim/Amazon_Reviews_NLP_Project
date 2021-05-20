## Amazon Product Reviews
### Question/Need:

Amazon lists millions of products across many categories. Choosing the right product on Amazon can often be a difficult, time-consuming decision that can often be undermined by the website's promotion of certain products, as well as false reviews.

I would like to explore whether or not an Amazon product review is true or fraudulent, and create recommendations based on overall review sentiment.

### Data:

Kaggle dataset of around 34,000 consumer reviews on Amazon, provided as a sample from Datafiniti's database.

The dataset consists of 21 features:
1. id
2. name
3. asins
4. brand
5. categories
6. keys
7. manufacturer
8. reviews.date
9. reviews.dateAdded
10. reviews.dateSeen
10. reviews.didPurchase
11. reviews.doRecommend
12. reviews.id
13. reviews.numHelpful
14. reviews.rating
15. reviews.sourceURLs
16. reviews.text
17. reviews.title
18. reviews.userCity
19. reviews.userProvince
20. reviews.username

These features will be subject to inclusion/exclusion based on further EDA.


I am also considering incorporating a dataset constructed by Xiang Zhang (xhiang.zhang@nyu.edu), which is a collection of ~35 million reviews across 18 years (up to March 2013).


### Tools:
* NLTK for NLP
* Pandas for data manipulation
* Matplotlib/Tableau for visualizations
* SKlearn for models and analysis
* SQLite for data storage in a db file

### MVP:
* For my MVP, I would like to process all of the review text and produce a sentiment analysis. Furthermore, I would also like to try and classify if a product review will be helpful or not, though I am unsure if this will be viable with the dataset. Additionally, I plan on exploring popular positive/negative mentions or phrases and their effect on the product's performance.
