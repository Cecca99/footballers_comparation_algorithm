# **Approach to find similar players to Francesco Acerbi**

This project is aimed at developing an approach to find 5 footballers most similar to a reference player. It involves the use of data manipulation tools , clustering techniques and calculation of Euclidean distances; the reference player will be Inter defender Francesco Acerbi.
The approach consists in:
* Data retrieval phase
* Data manipulation and preparation phase
* Clustering to group similar players
* Computation of euclidean distances between Acerbi and other players
* Visualization of the results


An application based on this approach has also been developed, allowing various defenders to be compared with Francesco Acerbi based on various statistics of the user's choice. It will give also a similarity score between the player chosen and Acerbi. It has been developed with *Streamlit*.

The application can be found at this link: [app](https://footballerscomparationalgorithm-hz5y4di5t2uuawexugz3ws.streamlit.app/)

All data refer to the 2022-2023 season and were retrieved from the *FBref* platform.
Some data about the players found refer to the 2023-2024 season and were scraped from *Transfermarkt*.

This repository is structured in the following way:

- **data:** This folder contains all data retrieved, manipulated, and used in the analysis. Specifically:
  - `5difenders_data.csv` Contains useful and up-to-date (2023-2024 season) data about the 5 players most similar to Acerbi.
  - `5difenders_list.pkl` Contains the list of 5 players most similar to Acerbi with personal data about the players such as team, position and year of birth.
  - `football_stats_2022_2023.pkl` Original dataframe retrieved from the *FBref* platform related to the 2022-2023 season.
  - `not_sorted_defenders.pkl` Players analysed and their stats.
  - `players.pkl` Data about all the players retrieved from *FBref* (no stats).
  - `sorted_defenders.pkl` Players analysed and their stats (sorted in a increasing way by their distance from Acerbi).
  - `sorted_defenders_nostats.pkl` Players analysed (sorted in a increasing way by their distance from Acerbi).
  - `stats_per_90_clean.pkl` Dataframe with all the stats of the player transformed in *per90* stats. It contains an index which indentifies each player univocally.

- **images:** This folder contains all the images used and developed throughout the project, comparation with players and clustering validation.
- **src:** Notebooks with the code developed during the project. All the work was done on Google Colab. Specifically:
  - `Data_Cleaning.ipynb` Code to clean, transform and prepare the data.
  - `Data_Retrieval.ipynb` Code developed to retrieve the data from *FBref*.
  - `Model.ipynb` Code used to normalize, cluster and compute distances between the data.
  - `Scraping_5Playersdata.ipynb` Code developed to scrape up-to-date data from *Transfermarkt* about the 5 players found.
  - `Visualization.ipynb` Code used to visualize radar charts and compare the players with Acerbi.
  - `radar_app.ipynb` Code used to develop and test the app.
- `app.py` Python code of the application.
- `app_functions.py` Useful functions to make the app work properly.
