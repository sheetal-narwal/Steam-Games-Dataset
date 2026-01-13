# Steam-Games-Dataset
The steam games dataset has been cleaned and analysed in this project.
The dataset contained information regarding game titles, publishers, developers, categories, genres, price, release date and so much more

## Data Cleaning
* The dataset contained game titles in various languages, which are translated using the GoogleTranslate function in Google Sheets. Other approaches such as translate, DeepL Translator and other python modules were used, but they were not efficient.
* Null values, duplicate values and Emojis were removed.
* The dataset contained some pecularities such as a game with 999.98 price. There pecularities were inspected.
* Dropped irrelevant columns such as additional content (contained mostly NA values) and required age.

## Data Analysis
* Categories and Genres of the games were exploded to create new columns.
* The correlation within categories and genres, and between them was visualized using a heatmap.
* Time Series analysis was conducted using Prophet library to understand game release frequency and obtain subsequent insights.
* Created wordclouds for the Action and Indie genres to analyse popularity within game titles.

## Insights
* There is indeed a game with a price tag of 999.98 available on Steam. The other pecularities were also inspected and kept in the dataset since they were found to be legitimate.
* Co-op, PvP, MMO and Cross-platform categories seem to be highly correlated indicating that games with these combinations are mode frequently developed.
* RPG & Adventure, Sports & Racing, Sports & Simulation seem to have a low positive correlation.
* Most games on the Steam platform were released after 2010, but Steam has included older games in their database as well (Earliest being from 1997)
* Most games are released on Thursdays and Fridays, contrary to the assumption that they are being released on weekends.
* Indie games seem to tend towards simulation, dungeons, war and adventure based themes, indicated by their importance in the wordcloud.
* Action games seem to tend towards zombies, adventure, space, battles and war based themes, indicated by their importance in the wordcloud. 
