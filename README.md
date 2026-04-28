# Music Finder IT 170 
- Authors: Alan, Caleb, Jacob, and Jonathan
- Project Music finder: This programs main function is to identify a song based on lyrics input by the user. It integrates many features such as Billboard chart data, Genius API validation, and speech recognition. 

# Features
- Search songs using lyrics input by user
- Finding the top three songs by an artist 
- Stores lyrics from Genius API
- Retrieves the top 100 songs from Billboard Top 100
- Automatically updates stored top 100 songs weekly
- Speech recognition for user inputs 
- Finding and printing the Album or song cover of a song.

# Project Structure
- List_of_Songs/ - Stores song lyrics
- Song_Info - Stores song data(artist, title, album)
- data.json - Serves as link between songs and info / lyric files
- loading_Songs.jpynb - Pulls and updates song data
- Structure.jpynb - Handles main program logic
- access_token.txt - Stores Genius api key

# Program Workflow
- Structure.jpynb - Main controller program. Handles user input, calls other modules, processes main flows of the program.
### Input Handling
- The user can provide input through typing or speaking
- When speech input is selected Structure.jpynb calls the speech recognition module found 'Speech Recognition' folder
- Speech renognition converts speech input through a microphone into text, then sends it to the main program
### Lyric Search Functionality
- The main program intakes the input and searches for matches inside of 'list_of_songs' file
- Utilizing the 'data.json file, this program matches lyrics with its corresponding song_data (artist, album, title) inside 'Song_Info'
- Output: This program displays the songs title, artist, album, and cover art.
### Top 3 Songs By Artist
- User enters the name of an Artist
- Program locates and displays the top three songs from Billboard data
### Automated Data Updates
- 'loading_Songs.jpynb' pulls the top 100 songs from Billboard
- Songs are verified using Genius API
- A recurring update takes place once a week to keep the top 100 songs up to date

# Group Responsibilities 
### Alan 
- Developed the main program structure, and implemented functions including:
- Search_song_by_lyrics():
- top_three() 
- display_results()
- Code for displaying song cover
### Caleb
- Implemented speech recognition feature inside Speech recog module
### Jonathan
- Designed (List_of_Songs) an organized structure of song data
- Created the 'loading_songs' module to automatically update Billboard top 100 songs
- Configured 'data.json' file
- Implemented and organized Songs_info file
### Jacob 
- Implemented a core main program function 'find_song_title()'
- Complied and finalized the README file 
