# Music Emotion Recognition
- Getting track information from Spotify using the Spotipy library.
  Link: https://github.com/spotipy-dev/spotipy
- An attempt at Music Emotion Recognition for the kaggle competition @ https://www.kaggle.com/competitions/kcl-artificial-intelligence-competition-22-23

# 🎵 Spotify Mood Dataset Generator 🎵
This project uses the **Spotipy** library to fetch track features from Spotify playlists categorized by mood. Whether you're a data scientist, music lover, or just curious about the science of sound, this dataset gives you insights into what makes a song feel happy, sad, chill, or angry.

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

![Screenshot 2025-03-15 154701](https://github.com/user-attachments/assets/806b0cc9-6ce8-43bc-b2e9-10d70401cd3f)
![Screenshot 2025-03-15 154650](https://github.com/user-attachments/assets/cfb1b9b4-1775-41ce-89a0-368b087c145d)
![Screenshot 2025-03-15 154639](https://github.com/user-attachments/assets/e49c3238-f95b-43c4-8a12-d03d7076b8ce)
![Screenshot 2025-03-15 154622](https://github.com/user-attachments/assets/ae9e6464-25dd-401f-a7ae-767d4e8305c0)
