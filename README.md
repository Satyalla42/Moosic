# 🎧 Moosic – Clustering Your Vibes

Can a machine learn your taste in music?

**Moosic** is an experimental project that uses unsupervised machine learning (K-Means clustering) to analyze and group your favorite songs based on audio features – then auto-generates playlists on Spotify that (maybe) match your vibe. The real question: can an algorithm beat your ears?

Listen to the results here 
https://open.spotify.com/playlist/1ZqXsDt0ScZ3Dl5yLG9N1R

---

## 🚀 Features

- 🔍 **Fetch tracks** from a Spotify playlist, saved tracks, or user listening history
- 📊 **Extract audio features** via Spotify's Web API (e.g. danceability, energy, tempo)
- 🤖 **Cluster tracks** using K-Means into mood-based or feature-based groups
- 🎵 **Generate new playlists** for each cluster and upload them to your Spotify account
- 👂 **Compare machine clusters vs. human taste** – can the algorithm predict your musical mood?

---

## 🧠 How It Works

1. **Authenticate** with your Spotify account (OAuth2)
2. **Collect songs** and extract their audio features using the Spotify API
3. **Normalize features** and apply K-Means clustering
4. **Group tracks** by cluster and label them (optional)
5. **Create playlists** on your Spotify with one click

---

## 🛠️ Tech Stack

- Python 3.10+
- `spotipy` – Spotify API wrapper
- `scikit-learn` – for K-Means clustering
- `pandas`, `numpy`, `matplotlib` – for data wrangling and visualization

---

## 🧪 Example Use Case

Cluster your liked songs into 4 groups:
```bash
python moosic.py --source liked --clusters 4
