# Music Finder IT 170 
Authors: Alan, Caleb, Jacob, and Jonathan
Project Music finder: This programs main function is to identify a song based on lyrics input by the user. It integrates many features such as Billboard chart data, Genius API validation, and speech recognition. 

# Features
-Search songs using lyrics input by user
-Finding the top three songs by an artist 
-Stores lyrics from Genius API
-Retrieves the top 100 songs from Billboard Top 100
-Automatically updates stored top 100 songs weekly
-Speech recognition for user inputs 
-Finding and printing the Album or song cover of a song.

#Project Structure
- List_of_Songs/ - Stores song lyrics
- Song_Info - Stores song data(artist, title, album)
- data.json - Serves as link between songs and info / lyric files
- loading_Songs.jpynb - Pulls and updates song data
- Structure.jpynb - Handles main program logic
- access_token.txt - Stores Genius api key
