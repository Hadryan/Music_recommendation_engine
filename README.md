# Music recommendation System
This project was done as my bachelor thesis in statistics at Lund University. This is a reasearch project and was not meant to be deployed in any other way.
All api info are removed, so to reproduce one would need to get their own api key from Spotify. The code is in notebooks, so the approach is more analytical and academic rather than actually deploying a recomender system. 

To read the paper, please visit: https://lup.lub.lu.se/student-papers/search/publication/9027165

## Collaborative filtering
Is done primarly in the collaborative_filtering.ipynb file. Here subsample from the millionsong dataset can be generated and used for various collaborative models.

## Content Based Filtering
### Playlists_dataset.ipynb
This notebook has functions that calls spotify's api and creates a dataset that is either composed of songs or playlists. Features for each song will also be included and they are used later on for content based models

### Content model
In content_model.ipynb the probibalistic content based model is created and evaluated. For detailed info regarding the methodology and reasoning behind computations I refer to my paper (link up top)

## Feature mapping
Since I couldn't get user info from spotifys api I used the approved millon song dataset which contains user info and then mapped each song with corresponding features from spotify's api. This is done in the feature_mapping.ipynb
