# Spotify Playlist Analyzer (AI/ML)

An AI/ML-powered web application that analyzes Spotify playlists to infer mood patterns from audio features.  
Built collaboratively with James McGhee, the project leverages Python, Spotipy, RapidAPI, and machine learning models to generate visual insights for playlists.  
This project started in OSU AI Club and evolved into a full-stack web application.



## Project Background

During development, we adapted to changes in Spotify's API, requiring a pivot in how the AI obtained audio features. This challenged us to creatively preprocess data and adjust our ML models to maintain functionality.  


## Core Website Features

- **Dynamic Playlist Display:** Pulls cover images and track info from Spotify, dynamically coloring pages based on dominant album artwork colors (Color Thief).  
- **Mood Prediction:** Backend ML models analyze audio features to infer playlist moods, visualized with pie charts.  
- **Search & Playlist Management:** Users can search playlists and submit new playlists, which are processed by the backend efficiently.


![Homepage](readme-imgs/home-page.png)  
Dynamic homepage with playlist search and submission features.

![Playlist Visualization](readme-imgs/hyper-playlist.png)  
Pages like this were created with user submissions of spotify playlist links, and page gets created showing ML-generated mood predictions and dynamic color backgrounds for the user.  

![Search Feature](readme-imgs/search-feature.png)  
Search functionality filters playlists dynamically based on user queries. Which looks at both playlist and song titles.




## Core Backend Features

- **ML Model:** Trained on 3,000 songs using a preprocessing pipeline to normalize audio features for pattern recognition. The model predicts moods based on features such as tempo, energy, and valence.  
- **Integration:** Backend connects the ML model with the frontend, processing Spotify playlists and returning insights in real time.  
- **Environment & Security:** `.env` files store sensitive API credentials (Spotipy, RapidAPI) to protect accounts and manage API usage.

<details>
<summary>Backend Structure</summary>

![Backend Structure](readme-imgs/structure.png)  
Directory layout and project structure for readability and maintainability.

![Model Structure](readme-imgs/ai-model.png)  
Overview of the AI/ML model repository and preprocessing workflow.

</details>


## Contributions

Calvin and James collaborated on all major aspects of this project. Key responsibilities included:

- **Calvin:** Data preprocessing, ML model integration, frontend dynamic visualizations.
- **James:** Model design, pattern recognition logic, charting, backend integration.



## Future Work

- Optimize backend processing speed for larger playlists.  
- Expand sorting and filtering features.  
- Explore additional ML-driven playlist insights and visualizations.
- Deploy website for constant use


