# spotify-lifetime-listening
## My seven years of Spotify history

Part one assembles the dataset of my personal listening history on Spotify from January 2015 to September 2022. 
I've supplemented that dataset with additional features about each track, artist, and album using Spotify's API. 

Part two cleans and visualizes the extracted data to better understand my listening history beyond the annual Spotify Wrapped.

Each row is one track.

### Documentation

- ts - The date and time the track was played
- ms_played	- How long the track was played in milliseconds
- master_metadata_track_name	- Track title
- master_metadata_album_artist_name	- Track artist
- master_metadata_album_album_name - Track album 
- spotify_track_uri(only in raw dataset) - The track's Uniform Resource Indicator from requested listening data
- reason_start - What action caused the track to being playing (the previous track ending, pressing the forward button, etc.)
- reason_end - What action caused the track to end playing (completing the track, unexpected exits, etc.)
- shuffle	- If shuffle mode was turned on 
- skipped	- If the track was skipped (1 for skipped, 0 for played-through)
- offline	- If the track was played offline (1 for offline, 0 for online)
- offline_timestamp	-  When a track was played offline, if used
- incognito_mode	- If private mode was turned on (1 for private, 0 for public)
- track_uri	- Track indicator extracted from Spotify's API
- album.uri	- Album indicator extracted from Spotify's API
- artists.uri	- Artist indicator extracted from Spotify's API 
- track_popularity - Track rating (0-100)
- duration_ms	- Length of the track in milliseconds
- album.album_type - Whether the track was a part of an album, a single, collection, etc. 
- album.release_date - Release year in cleaned dataset (raw data includes a mix of date formats)
- genres	- List of associated genres with the track
- artist_popularity	- Artist rating (0-100)
- followers.total	- Number of artist followers
- album_popularity - Album rating (0-100)
- label	- Record label behind the track
- tracks.total - Number of tracks on the album	
- danceability	- Measured from 0-1 (least to most danceable)
- energy - Measured from 0-1 (least to most intensity)	
- key	- 12 keys from 0 to 11
- loudness - Measured in decibles
- mode	- 1 for major and 0 for minor
- speechiness	- Measured from 0-1 (lowest to highest presence of talking)
- acousticness - Measured from 0-1 (least to most acoustic)
- instrumentalness	- Measured from 0-1 (highest to lowest detection of vocals)
- liveness	- Measured from 0-1 (least to most audience presence in the recording)
- valence	- Measured from 0-1 (lowest to highest positivity)
- tempo	- Measured in beats per minute
- time_signature - Number of beats per measure
