# Museam-Fond
Training AI to recognize the type or category of a museum item when a new item is added to the catalog.


# Description
This project based on [All_Cups hackathon](https://cups.mail.ru/ru/tasks/1087).  

**Practice Skills:**
-  Classification foto data;
-  Classification text data;

# Goal
It was necessary to determine the category of the object of the museum fund by the description or image.   
**I worked only with description.**

# Data
All data information in [directory](/data).
Additional training sample - [train_url_only.csv](/data/train_url_only.csv).
The additional sample is characterized by a significantly larger amount of data on the number of items, but there are no image files for them, but they can be obtained from the links stored in the url column.  

The [main source of data] is the FGIS «Gosudarstvennogo kataloga Muzejnogo fonda Rossijskoj Federatsii». Data collection occurs automatically through the internal information systems of the Ministry of Culture of Russia.(https://opendata.mkrf.ru/opendata/7705851331-museum-exhibits).

# Score
F1-score

## [Baseline](/house_prices_preprosesing.ipynb)
As basemodel was using [LogisticRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html). 
Score - 0.6300774414141161.
## [Model](/house_prices_model.ipynb)
As main model was using [XGBClassifier](https://xgboost.readthedocs.io/en/latest/python/python_api.html).
# Final Score
Score 0.8933173131540203
