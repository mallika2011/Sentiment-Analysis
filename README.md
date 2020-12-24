# Sentiment-Analysis

Building a text classification model using BERT and pytorch for sentiment analysis. 

The model is trained and built for a corpus of ***Google Play Reviews***. The dataset has been scraped using the ```google_play_scraper``` library. The models can be found on my google drive, and are not uploaded here due to space constraints.

## Directory Structure
```
.
│   README.md
|   LICENSE
│   dataset-scraper.ipynb
│   text-preprocessing.ipynb
│   text-classification-bert.ipynb
│
└───data
│   │   apps.csv
│   │   reviews.csv
│   │
│   
└───models
    │   model.bin
    │   model_base_cased_state_842.bin
    │   model.pth
```

### Usage

* The ```dataset-scraper.ipynb``` notebook has all the code required to scrape the reviews dataset
* The ```text-classification-bert.ipynb``` is the final notebook that has the code required to run the classification model.

## Performance 

Below are the performance metrics of the classification model

|precision  |  recall  |f1-score   |support|
|----------|:---------:|--------:|------:|
   | negative     |  0.83   |   0.80    |  0.81   |   257|
   |  neutral     |  0.75    |  0.75     | 0.75   |    253|
   | positive      | 0.85     | 0.88      |0.86       |308|
 |   accuracy       |     -      |    -     |0.81    |   818|
 |  macro avg      | 0.81    |  0.81 |     0.81    |   818|
 |weighted avg   |    0.81    |  0.81    |  0.81  |     818|
 |
