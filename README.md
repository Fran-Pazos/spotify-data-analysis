# Spotify Data Analysis

## Overview

This project performs an Exploratory Data Analysis (EDA) of a Spotify dataset containing 41,106 tracks from different decades, ranging from the 1960s to the 2010s.

The main objective is to explore the musical characteristics associated with song popularity and identify which features have the strongest relationship with the target variable.

## Dataset

The dataset contains information about Spotify tracks and their musical characteristics.

Some of the main variables analyzed are:

- `danceability`: how suitable a track is for dancing
- `energy`: intensity and activity of the track
- `valence`: the musical positivity or happiness conveyed by a track
- `tempo`: tempo of the track
- `loudness`: overall loudness of the track
- `duration_ms`: track duration in milliseconds
- `target`: popularity classification (0 = not popular, 1 = popular)
- `decade`: decade associated with the track

The complete dataset contains 20 variables.

## Tools and Technologies

- Python
- Pandas
- Seaborn
- Matplotlib
- Jupyter Notebook

## Analysis

The analysis includes:

- Dataset exploration
- Data type inspection
- Descriptive statistics
- Missing value detection
- Distribution analysis
- Outlier detection using boxplots
- Correlation analysis
- Comparison of musical features between popular and non-popular tracks
- Data visualization

## Key Findings

The analysis produced several relevant findings:

- No missing values were found in the dataset.
- `danceability`, `energy` and `valence` showed left-skewed distributions, with most values concentrated between approximately 0.2 and 0.8.
- Outliers were identified, particularly in `energy`, and to a lesser extent in `danceability` and `valence`.
- `danceability` showed the strongest correlation with the target variable (0.35).
- `valence` showed a weaker positive correlation with the target variable (0.25).
- `energy` had a lower correlation with the target variable (0.18).
- Popular tracks tended to have higher levels of danceability and valence.
- The difference in energy between popular and non-popular tracks was less pronounced.

These results suggest that danceability and valence have a stronger relationship with song popularity than energy in this dataset.

## Project Structure

```text
spotify-data-analysis/
│
├── Spotify_Analysis.ipynb
├── spotify_dataset.csv
└── README.md
