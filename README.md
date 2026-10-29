# Steam Games Analysis

## Dataset

Dataset used: Steam games Dataset 2025  
Link: https://www.kaggle.com/datasets/srgiomanhes/steam-games-dataset-2025

## Data Cleaning

- Dropped additional_content column as it was not needed by using the df.drop() function.
- Fixed a problem where some release_dates also included time of day by using df.replace().
- Split release_dates into 3 columns which are year, month, and day by using dt.year, dt.month, and dt.day and assigned appropriate data types to them.
- Exploded the columns “Categories”, and “Genres” for easier analysis using df.explode().
- Removed missing values from columns “Categories”, and “Genres” while analyzing them.
- Turned column “platform” into 3 dummy columns for easier analysis by using df.get_dummies().

## Visualizations

![Bar chart](<Visualizations/number of singe player, multiplaye, and co-op games.png>)

Bar chart to show the number of games on Steam that support single player, multiplayer, and co-op modes.

Multi-line chart showing the number of games on steam that supports the different game modes over the years between 2011 and 2024.

![Multi-line chart](<Visualizations/number of game modes on steam over time.png>)

Word Cloud showing the most common genres for steam games.

![Word Cloud](<Visualizations/Genre Word Cloud.png>)

Pie charts showing the proportion of games on Steam that support different operating systems (Windows, Linux, and Mac).

![Pie charts](<Visualizations/Support for different OS.png>)

Line chart showing the average price of a Steam game from 2011 to 2024.

![Line chart](<Visualizations/avg price.png>)
