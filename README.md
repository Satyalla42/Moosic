# 🎧 Moosic – Clustering Your Vibes

Can a machine learn taste in music?

**Moosic** is an experimental project that uses unsupervised machine learning (K-Means clustering) to analyze and group songs based on audio features – then auto-generates playlists on Spotify that match the vibe. The real question: can an algorithm beat your ears?


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

Listen to the results here 
https://open.spotify.com/playlist/1ZqXsDt0ScZ3Dl5yLG9N1R
https://open.spotify.com/playlist/0b0AScx4L8ut23Loyl3K7R
https://open.spotify.com/playlist/4CWrXzih8R4CdYYZ6raD94
https://open.spotify.com/playlist/5oDiFC5VOmN8L97iuiOHCi
https://open.spotify.com/playlist/4mMMxKZdmREB7wk9ZOmLdw
https://open.spotify.com/playlist/5e1k9cYi5cQl4XRjzGp086
https://open.spotify.com/playlist/5XZO1RJE3SJKqmXu4NDi1h
https://open.spotify.com/playlist/2DSDdGSEB3XSjdZEM2mJQN
https://open.spotify.com/playlist/4pSqQRx4TItI7tyPUhXrh7
https://open.spotify.com/playlist/5hkptRluweqWPyYporXc2F
https://open.spotify.com/playlist/7H4S8xUvNOIJoKwA5J9TPi
https://open.spotify.com/playlist/2jNe1a4VsCbEkzB9gtEYaq
https://open.spotify.com/playlist/1s6eUmiCIS0C6KEw6JaOyu
https://open.spotify.com/playlist/30TeawIdR40TLg9t1KnCea
https://open.spotify.com/playlist/6ITXU25ZautkH5Sz7nOrVY
https://open.spotify.com/playlist/2E0RoVgd6i99nMjCNcRD1y
https://open.spotify.com/playlist/34JskIAVBfgFJG1NixGVck
https://open.spotify.com/playlist/7sygLrSqBjdHWjPfs65QAY
https://open.spotify.com/playlist/0aBySxxhtFM82ssgRU9mAh
https://open.spotify.com/playlist/0hyqx0kIDnz7zrhkM0otVb
https://open.spotify.com/playlist/6qzKqXxcXIpR9TVwlIfEPr
https://open.spotify.com/playlist/3yh21HZ9uN7NoxzfTARY1O
https://open.spotify.com/playlist/1p54vovYAZu8oG7YUivEnG
https://open.spotify.com/playlist/1M1pzvS4BlxFdL0AJ55H4j
https://open.spotify.com/playlist/5rIykjcwnNFmlLMRsMkVCg
