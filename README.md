# Exploratory Data Analysis: Zomato Restaurants

EDA of the Zomato Restaurants dataset from Kaggle using Python, Pandas, Matplotlib and Seaborn.

## Dataset
- **Source:** <paste your Kaggle dataset link here>
- **Size:** 9,551 restaurants x 21 columns (mixed numeric, categorical, geographic)
- **Each row:** one restaurant, with location, cuisines, cost, price range, booking/delivery flags, rating and votes
- **File:** `Zomato_Restaurant_Dataset.csv`

## Questions explored
1. How are ratings distributed?
2. Which cuisines are most common, and which score highest?
3. Do online delivery or table booking relate to ratings?
4. Do pricier restaurants get better ratings?
5. Are ratings linked to number of votes?
6. How do cities compare on volume and cost?
7. Which numeric variables are correlated?

## Contents
- `eda_notebook.ipynb`: the full analysis, with interpretation after each chart and a findings summary
- `Zomato_Restaurant_Dataset.csv`: the data

## Run it
```
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook eda_notebook.ipynb
```

## Key findings
- The median rating is 3.4 and only about 4% of rated restaurants reach 4.5+.
- The most common cuisines (North Indian, Chinese, Fast Food) are not the best rated; Italian, American and Continental average about 3.7-3.8.
- Median rating rises with price range (3.2 -> 3.9), and restaurants with table booking rate higher (3.6 vs 3.4), while online delivery makes no difference.
- Votes are the numeric variable most strongly related to rating (Spearman 0.68).
