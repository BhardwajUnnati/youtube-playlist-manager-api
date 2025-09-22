# YouTube Playlist Manager — Jupyter Notebook

A single Jupyter notebook to authenticate with YouTube (OAuth 2.0), create a playlist, search top results for song queries, add them, list/delete items, and log inputs.

## Features
- OAuth sign-in (stores `token.json` locally)
- Create playlist (private by default)
- Search & add top video match for each song
- List/delete items in playlist
- Save inputs to `logs/playlist_YYYY-MM-DD.txt`

## Quickstart
1. **Install dependencies**:
   ```bash
   python -m venv .venv && . .venv/bin/activate   # Windows: .venv\Scripts\activate
   pip install -r requirements.txt

2. Get Google OAuth credentials
- Go to Google Cloud Console
- Create an OAuth 2.0 Client ID (Desktop App)
- Download as client_secret.json and put it in your local project folder.
- ⚠️ Do not commit this file to GitHub.

3.Run the notebook
- Open YouTube_Playlist_Manager.ipynb
- Run cells in order: Setup/Auth → Create Playlist → Add Songs → List/Delete.
- Follow prompts (playlist name, description, songs).

4.Output
- Final cell prints your playlist URL.
- Input snapshot saved to logs/playlist_YYYY-MM-DD.txt.
