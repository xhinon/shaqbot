
# Discord Chat Bot
***  
This is a simple Node.js based chat and music bot for Discord.

__The music commands are:__
* `play <url>|<search string>`: Play audio from YouTube.
* `search <search string>`: Search's for up to 10 videos from YT.
* `skip [number]`: Skip a song or multi songs with skip [some number].
* `queue [position]`: Display the current queue.
* `pause`: Pause music playback.
* `resume`: Resume music playback.
* `remove [position]`: Remove a song from the queue by position.
* `volume`: Adjust the playback volume between 1 and 200.
* `leave`: Clears the song queue and leaves the channel.
* `clearqueue`: Clears the song queue.
* `np`: Show the current playing song.  



__Permissions:__  
* If `anyoneCanSkip` is true, anyone can skip songs in the queue.
* If `anyoneCanAdjust` is true, anyone can adjust the volume.
* If `ownerOverMember` is true, the set ID of the user (`ownerID`) will over-ride permissions from the bot.

***
# Installation
***  

__Installation:__  
* `npm install`  

# Options & Config.
***

## Basic variables.
| Option | Type | Description | Default |  
| --- | --- | --- | --- |
| youtubeKey | String | A YouTube Data API3 key. Required to run. | NaN |
| botPrefix | String | The prefix of the bot. Defaults to "!". Can also be a Map of prefix's. | ! |
| ownerOverMember | Boolean | Whether the owner over-rides `CanAdjust` and `CanSkip`. | false |
| ownerID | String | The ID of the Discord user to be seen as the owner. Required if using `ownerOverMember`. | NaN |
