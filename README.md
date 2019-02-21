# ETL Project - World Happiness Compared with other Metrics
#### The purpose of this ETL Project was to find different datasets including a variety of metrics on certain countries and comparing them with their happiness index.
##### The datasets used to create final csv file are:
- Happiness: https://data.world/laurel/world-happiness-report-data/workspace
  - This dataset includes the happiness index as a result of other data about specific countries including social support, life expectancy, confidence in government, etc.
- Freedom: https://www.kaggle.com/gsutters/the-human-freedom-index
  - This dataset includes scores of Personal, Economic, and Human freedom based on data about certain countries like security and safety, freedom of religion/expression/organization, legal system/property rights, etc.
- Income: https://www.kaggle.com/worldbank/world-development-indicators#Series.csv
  - This dataset includes indicators of development in certain counties
  - The only useful data I pulled from this was the Income Group column stating each country's economic status
- Suicide: https://www.kaggle.com/russellyates88/suicide-rates-overview-1985-to-2016/version/1
  - This dataset includes suicide rates among countries based on sex and age group.
  - I combined the populations of all age groups and split between sex, finding the number of suicides per 100,000 people
##### Steps to create final csv file:
- Filter every dataset for the year 2015
- Pulled desired metrics from each dataset to be included in final csv file
- Clean datasets by dropping all rows with NaN in them
- Combine all cleaned datasets on 'Country' columns
- Export combined dataset in csv file
