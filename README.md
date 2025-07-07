# Music Emotion Recognition
- Getting track information from Spotify using the Spotipy library.
  Link: https://github.com/spotipy-dev/spotipy
- An attempt at Music Emotion Recognition for the kaggle competition @ https://www.kaggle.com/competitions/kcl-artificial-intelligence-competition-22-23

# 🎵 Spotify Mood Dataset Generator 🎵
This project uses the **Spotipy** library to fetch track features from Spotify playlists categorized by mood. 

# What's in the Dataset?
The generated dataset consists of track features that describe the audio properties of songs. Here’s what each column means:

⚡ energy – Intensity of a song (0 to 1). More energy = more power!  
🎤 liveness – Is it live or studio? Higher values mean a live audience presence.  
🏃 tempo – Beats per minute (BPM). Faster songs = more movement!  
🗣️ speechiness – How much speech is in the track?  
🎸 acousticness – Higher means more acoustic, lower means more electronic.  
🎶 instrumentalness – Measures the presence of vocals. Close to 1? Probably an instrumental.  
💃 danceability – Can you groove to it? Higher values mean it’s dance-floor-ready!  
⏳ duration_ms – Track length in milliseconds.  
🔊 loudness – Measured in dB, higher is louder.  
😊 valence – How happy or sad a song feels (0 = sad, 1 = happy).  
🎭 mood – The mood label (happy, sad, angry, chill).  

# Models Used:

**Random Forest Classifier (RFC)**: n_estimators=100, max_depth=None, random_state=42  
**XGBoost Classifier**: n_estimators=100, max_depth=6, learning_rate=0.1, objective='multi:softmax'  
**Naïve Bayes Classifier**: GaussianNB() from sklearn.naive_bayes  

# Results
XGBoost performs better, achieving a more balanced class distribution and fewer misclassifications.  
Random Forest, while effective, struggles with certain classes, leading to a higher rate of incorrect predictions.  
If prioritizing accuracy and balanced performance → XGBoost is the better choice.  

Class 0: Represents Angry or high-energy, intense emotions.
Class 1: Represents Happy or upbeat, positive emotions.
Class 2: Corresponds to Sad or melancholic emotions.
Class 3: Represents Chill or relaxed, soothing emotions.

![Screenshot 2025-03-15 154622](https://github.com/user-attachments/assets/eca7d2a3-4490-4eea-b88e-43d6a566de47)
![Screenshot 2025-03-15 154639](https://github.com/user-attachments/assets/bb0cf192-4bd9-4233-a8d4-9fad4b68b01b)
![Screenshot 2025-03-15 154701](https://github.com/user-attachments/assets/9b3fa6dd-18c9-49fb-89fd-da9602f8747b)
![Screenshot 2025-03-15 154650](https://github.com/user-attachments/assets/8c37edde-8aa2-470c-9147-121fb5256cbe)
