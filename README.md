# Movies-ETL

To automate this Movies ETL pipeline, we have to assume that movies do not have "episodes" related to them; only TV shows have "episodes" so we have to drop any inputes with "episodes".
We also make the assumption that the titles given by the Kaggle data are more complete and consistant than the titles given by wikipedia, so we drop the wikipedia titles.
Another assumption we make is that the runtime data from Kaggle are more complete and any data we do not get from the Kaggle data will be filled with Wikipedia's runtime data.
By comparing the budget information from wikipedia and kaggle we notice that there are more outliers in the wikipedia data whereas the kaggle data shows a few missing data. We choose to fill in the missing kaggle data with wikipedia's data.
