# TripAdvisor sentiment analysis

## Introduction
Sentiment analysis task performed on text reviews scraped from the Italian TripAdvisor website. The project is relative to the final chellenge of the *Data Science Lab* course in the Data Science and Engineering MSc at Politecnico di Torino, A.A. 2019/2020.

## Organization
The code in the [Python notebook](./main.ipynb) is organized in four main sections:

- data exploration
- data preprocessing
- algorithmic choice
- tuning and validation

All details can be found in the project [report](./report.pdf).

## Dataset
Training and validation datasets are composed of text reviews of hotels in Italian language, in `csv` files with `pos` or `neg` labels. Additional reviews (contained in [`data/external.csv`](./data/external.csv)) are scraped using an external [TripAdvisor scraper](https://github.com/gabridego/tripadvisor-scraper) and used for model training.

## Dependencies

- [scikit-learn](https://scikit-learn.org/stable/index.html) for machine learning model
- [pandas](https://pandas.pydata.org/) and [NumPy](https://numpy.org/) for data handling
- [matplotlib](https://matplotlib.org/), [seaborn](https://seaborn.pydata.org/) and [word_cloud](https://amueller.github.io/word_cloud) for visualization
- [NLTK](https://www.nltk.org/) and [spaCy](https://spacy.io/) for text processing
- [spacy-langdetect](https://github.com/Abhijit-2592/spacy-langdetect) to detect the actual language of the reviews
- [py-googletrans](http://py-googletrans.rtfd.io/) to translate non-Italian reviews