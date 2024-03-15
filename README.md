# **Approach to find similar players to Francesco Acerbi**

This project is aimed at developing an approach to find 5 footballers most similar to a reference player. It involves the use of data manipulation tools , clustering techniques and calculation of Euclidean distances; the reference player will be Inter defender Francesco Acerbi.

An application based on this approach has also been developed, allowing various defenders to be compared with Francesco Acerbi based on various statistics of the user's choice. It will give also a similarity score between the player chosen and Acerbi.

The application can be found at this link: [app](https://footballerscomparationalgorithm-hz5y4di5t2uuawexugz3ws.streamlit.app/)

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



