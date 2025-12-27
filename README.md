# Spotify-Data-Analysis
End to End Data Analysis and Machine Learning Project

## Project Overview 
This project presents a comprehensive, end-to-end analysis of factors influencing song popularity on Spotify, combining data analytics, statistical reasoning, and machine learning. The focus was not only on predicting popularity scores, but also on understanding what truly drives audience engagement, making this project highly relevant for data analytics, product analytics, and business decision-making roles.

## Business Problem
Music streaming platforms rely heavily on understanding user preferences to:
1. Improve playlist curation.
2. Support artist promotion strategies.
3. Enhance user engagement and retention.

The goal of this project was to:
1. Predict Spotify song popularity scores (0–100).
2. Identify key audio and metadata features driving popularity.
3. Translate analytical findings into actionable insights for content and product teams.

## Dataset Description
a. Source: Kaggle (Spotify Dataset)
b. Size: 114,000+ tracks
c. Features: 21 audio and metadata attributes, including:
1. track_id: The Spotify ID for the track
2. artists: The artists' names who performed the track. If there is more than one artist, they are separated by a ;
3. album_name: The album name in which the track appears
4. track_name: Name of the track
5. popularity: The popularity of a track is a value between 0 and 100, with 100 being the most popular. The popularity is calculated by algorithm and is based, in the most part, on the total number of plays the track has had and how recent those plays are. Generally speaking, songs that are being played a lot now will have a higher popularity than songs that were played a lot in the past. Duplicate tracks (e.g. the same track from a single and an album) are rated independently. Artist and album popularity is derived mathematically from track popularity.
6. duration_ms: The track length in milliseconds
7. explicit: Whether or not the track has explicit lyrics (true = yes it does; false = no it does not OR unknown)
8. danceability: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable
9. energy: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale
10. key: The key the track is in. Integers map to pitches using standard Pitch Class notation. E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on. If no key was detected, the value is -1
11. loudness: The overall loudness of a track in decibels (dB)
12. mode: Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0
13. speechiness: Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks
14. acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic
15. instrumentalness: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content
16. liveness: Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live
17. valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry)
18. tempo: The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration
19. time_signature: An estimated time signature. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure). The time signature ranges from 3 to 7 indicating time signatures of 3/4, to 7/4.
20. track_genre: The genre in which the track belongs

## Methodology (End-to-End Workflow)
### Data Cleaning & Preprocessing
1.Handled missing values and duplicate records
2. Performed categorical encoding where required
3. Applied feature scaling for model stability
4. Conducted multicollinearity checks to ensure reliable regression results

### Exploratory Data Analysis (EDA)
1. Analyzed distributions of audio features
2. Visualized relationships between popularity and key variables
3. Identified patterns indicating how musical characteristics influence listener engagement

### Statistical Analysis
1. Conducted correlation analysis to identify influential features
2. Applied hypothesis testing to validate relationships
3. Ensured statistically sound feature selection before modeling

### Model Building
#### Developed and compared multiple regression models:
1. Linear Regression
2. Ridge Regression
3. Lasso Regression
4. Ensemble Models (Random Forest, Gradient Boosting, AdaBoost)
5. XGBoost (best-performing model)

### Model Evaluation
1. Evaluated models using R² score
2. XGBoost achieved an R² value of 0.70, indicating strong explanatory power for popularity prediction
3. Compared model performance to select the most reliable approach

## Key Insights (Business Value)
1. Danceability, energy, and valence emerged as the strongest predictors of popularity
2. Songs with higher energy and positive emotional tone tended to perform better
3. Audio features play a measurable role in shaping listener engagement and content success

#### These insights can directly support:
1. Playlist ranking algorithms
2. Artist marketing strategies
3. Data-driven content recommendations

## Results & Impact
1. Built a reliable regression model to predict song popularity
2. Delivered interpretable insights linking audio features to engagement
3. Demonstrated strong capabilities in:
a. Data preprocessing
b. Statistical reasoning
c. Model evaluation
d. Business-oriented insight generation
