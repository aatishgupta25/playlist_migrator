# playlist_migrator

# Spotify to YouTube Playlist Migrator
This project allows you to migrate your Spotify playlists to YouTube, creating a new YouTube playlist with corresponding videos for each track.
## Features
- Authenticate with Spotify and YouTube APIs
- Fetch tracks from a specified Spotify playlist
- Search for corresponding YouTube videos
- Create a new YouTube playlist
- Add found videos to the new YouTube playlist
## Prerequisites
- Python 3.6+
- Spotify Developer Account
- Google Developer Account with YouTube Data API v3 enabled
## Installation
1. Clone this repository:
git clone [https://github.com/aatishgupta25/spotify-to-youtube-migrator.git](https://github.com/aatishgupta25/playlist_migrator)
cd spotify-to-youtube-migrator
2. Install required packages:
pip install spotipy google-auth-oauthlib google-api-python-client
3. Set up your Spotify and YouTube API credentials:
- For Spotify: Create an app in the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/) and note your Client ID and Client Secret.
- For YouTube: Create a project in the [Google Developer Console](https://console.developers.google.com/), enable the YouTube Data API v3, and download the client configuration file.
## Usage
1. Open the script and replace the following placeholders:
- `SPOTIPY_CLIENT_ID`: Your Spotify Client ID
- `SPOTIPY_CLIENT_SECRET`: Your Spotify Client Secret
- `SPOTIPY_REDIRECT_URI`: Your Spotify Redirect URI (e.g., 'http://localhost:8888/callback')
- `# Insert your Spotify playlist ID here`: Your Spotify playlist ID
- `# Insert your desired YouTube playlist name here`: Your desired YouTube playlist name
- `# Insert your desired YouTube playlist description here`: Your desired YouTube playlist description
2. Run the script:
python playlist_migrator.py
3. Follow the prompts to authenticate with Spotify and YouTube:
- For Spotify: Click the provided link, log in, and paste the redirected URL back into the console.
- For YouTube: Click the provided link, log in, and paste the authorization code back into the console.
- Your Spotify playlist ID
- Your desired name for the new YouTube playlist
- A description for the new YouTube playlist
4. The script will then migrate your playlist, creating a new YouTube playlist with corresponding videos.
## Note
This script uses API calls to both Spotify and YouTube. Be aware of rate limits and potential quota restrictions, especially for larger playlists.
