# Music Emotion Recognition
- Getting track information from Spotify using the Spotipy library.
  Link: https://github.com/spotipy-dev/spotipy
- An attempt at Music Emotion Recognition for the kaggle competition @ https://www.kaggle.com/competitions/kcl-artificial-intelligence-competition-22-23

# 🎵 Spotify Mood Dataset Generator 🎵
This project uses the **Spotipy** library to fetch track features from Spotify playlists categorized by mood. Whether you're a data scientist, music lover, or just curious about the science of sound, this dataset gives you insights into what makes a song feel happy, sad, chill, or angry.

# What's in the Dataset?
The generated dataset consists of track features that describe the audio properties of songs. Here’s what each column means:

energy – Intensity of a song (0 to 1). *More energy = more power!*
liveness – Is it live or studio? *Higher values mean a live audience presence.*
tempo – Beats per minute (BPM). *Faster songs = more movement!*
speechiness – How much speech is in the track?
acousticness – Higher means more acoustic, lower means more electronic.
instrumentalness – Measures the presence of vocals. Close to 1? Probably an instrumental.
danceability – Can you groove to it? *Higher values mean it’s dance-floor-ready!*
duration_ms – Track length in milliseconds.
loudness – Measured in dB, higher is louder.
valence – How happy or sad a song feels (0 = sad, 1 = happy).
mood – The mood label (happy, sad, angry, chill).

