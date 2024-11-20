# Spotify to MP3 Downloader

A Python-based tool that downloads songs and playlists from Spotify as MP3 files with complete metadata and album artwork.

## Features

- Download individual Spotify tracks or entire playlists
- Preserves complete metadata including:
  - Artist information
  - Album name
  - Track title
  - Release date
  - Track number
  - ISRC code
  - Album artwork
- Handles duplicate files with options to skip or replace
- Progress tracking for playlist downloads
- Downloads audio in high quality MP3 format
- Support for public Spotify playlists

## Prerequisites

- Python 3.7+
- Spotify Developer Account credentials
- Internet connection

## Installation

1. **Clone the Repository**

2. **Set Up Virtual Environment**

# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate

3. **Install Dependencies**

pip install -r requirements.txt

4. **Set Up Spotify API**

# Windows
set SPOTIPY_CLIENT_ID=your_client_id
set SPOTIPY_CLIENT_SECRET=your_client_secret

# macOS/Linux
export SPOTIPY_CLIENT_ID='your_client_id'
export SPOTIPY_CLIENT_SECRET='your_client_secret'

## Running the Application

1. **Start the Program**

python project.py

2. **Enter Spotify URL**
   - For a single track:

Enter a spotify url: https://open.spotify.com/track/1234...

   - For a playlist:

Enter a spotify url: https://open.spotify.com/playlist/1234...

3. **Handle Duplicates**
   When a file already exists, you'll see these options:
   - `R` - Replace current file
   - `RA` - Replace all existing files
   - `S` - Skip current file
   - `SA` - Skip all existing files

4. **Find Your Downloads**
   - Downloaded files are saved in the `music` directory
   - Files include complete metadata and artwork
   - Format: `Artist - Title.mp3`

## Common Issues

1. **Clone Errors**
   - Ensure Git is installed
   - Check internet connection
   - Verify repository URL

2. **Virtual Environment Issues**

# Reset virtual environment
deactivate  # if already in a venv
rm -rf venv  # or 'rmdir venv /s /q' on Windows
python -m venv venv

3. **Permission Problems**

# Windows (Run as Administrator)
python -m pip install --user -r requirements.txt

# Linux/macOS
sudo pip install -r requirements.txt

4. **API Authentication**
   - Double-check credentials
   - Verify environment variables
   - Ensure Spotify Developer account is active

## Tips for Success

1. **Before Running**
   - Ensure stable internet connection
   - Check available disk space
   - Verify API credentials

2. **During Downloads**
   - Don't interrupt the process
   - Monitor download progress
   - Check the tmp folder regularly

3. **After Completion**
   - Verify downloaded files
   - Check metadata accuracy
   - Clear tmp directory if needed

## Maintenance

- Keep dependencies updated
- Monitor API usage limits
- Clear temporary files regularly
- Back up your credentials

## Getting Help

If you encounter issues:
1. Check the error message
2. Verify your setup
3. Review common issues above
4. Create a detailed issue report

Remember to never share your API credentials when seeking help!
