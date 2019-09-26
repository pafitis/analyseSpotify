# analyseSpotify

Exploring my music taste through Spotify data.

### Setup: 

People ask me what type of music I am into. This always turns to "Oh you like techno?", which in turn I reply "Yes, but specific types". This analysis will hopefully enlighten me with the differences of my favourite techno playlist and my not-so-favourite Spotify-made playlist Techno Bunker.

### Downloading data:

I have used the great webapp to download a csv version of my playlist. Check it out here http://static.echonest.com/SortYourMusic/

### Exploratory analysis of personal playlist:

This is what my playlist looks like:
![image](https://user-images.githubusercontent.com/44204113/65709832-a8e17500-e089-11e9-92d7-b5eb9529a272.png)

#### Basic exploration of distributions:
![distro](https://user-images.githubusercontent.com/44204113/65709971-efcf6a80-e089-11e9-8db8-20a1466ca6e5.png)

#### Descriptive statistics:
![image](https://user-images.githubusercontent.com/44204113/65710000-feb61d00-e089-11e9-8bd0-31584eb7336c.png)

#### Correlation plots (not all of them):

![corr_en_loud](https://user-images.githubusercontent.com/44204113/65710589-396c8500-e08b-11e9-9791-91d67b18fee8.png)

![corr_en_pop](https://user-images.githubusercontent.com/44204113/65710590-396c8500-e08b-11e9-852d-7bd83fc1d5d4.png)

![corr_en_val](https://user-images.githubusercontent.com/44204113/65710592-396c8500-e08b-11e9-8094-c82ddd30fc7c.png)

#### Similarity graph (t-SNE) of 'Drexciya' songs
![drexciya](https://user-images.githubusercontent.com/44204113/65710225-7a17ce80-e08a-11e9-9e67-5eeba191316e.png)

### Personal vs Spotify
![tfnsvstechnobunker](https://user-images.githubusercontent.com/44204113/65710756-86e8f200-e08b-11e9-87ca-4d146a361e4f.png)


***Blue** represents music from my personal playlist. **Orange** represents music coming from the "Techno Bunker" playlist*


## Inference
#### Similarities:

- Year of Release: 
    - This makes sense, both from my personal taste as well as the kind of techno artist that are available on Spotify. Many old school artists are not available on the platform (not all but a few) hence you end up listening to mostly newly released songs (past 5 years)
- Seconds:
    - Again, most techno songs follow the same pattern. Long build-up, breakdown, build-up, end. This usually runs around 6-8 minutes. This confirms the two bell shapes. Notice mine (blue) has a long leg indicating some songs run for more than 13 minutes. Hey Ricardo Villalobos!
- Acoustic-ness:
    - Pretty self-explanatory. This is an analysis on techno playlists!


#### Differences:
- BPM:
    - Although there's a big overlap between the two shapes, it seems that I prefer slower songs with the exception of sometimes going crazy, with tracks having 170-190 BPMs. There's greater dispersion in my tracks indicating that my playlist features tracks from wider backgrounds (chicago, london, ...)
- Energy, Loudness, Dancability:
    - Especially interesting here.
    - Although my songs range to higher BPM values, my tracks are ranked with lower Energy metrics. Might be counterintuitive at first but this can be a consequence of the subjective measurement of "energy". Some could consider "darker" or repeatitive sounds to be less energetic? We can't know exactly unless there is a specification on how Spotify ranks that. 
    - Loudness follows the same pattern. I can see how I rank lower though. I prefer more monotonous or "minimal" sounds which usually aren't the loudest. When I think loud, Amelie Lens comes to mind. That's not what is typically in my playlist (although she is good).
    - Here we see a complete switch! Even if I ranked low on energy and loudness, it seems that my songs are dance-indusers! Partyyyy.
- Valence:
    - A measurement of "happyness". Don't know if we should be taking it into consideration given how ambiguous any "happyness" measurements are in the first place but more specifically when considering techno songs. Regardless, if we do so then I'm happier than your average techno-head. Take that.
- Popularity:
    - Not to brag or anything... but the graph speaks for itself.
    


**Tl;dr: I like techno songs that are slightly slower, less aggressive in terms of loudness and generally more dancable. It seems that I also have a hunch for "happy" techno whatever that means... The classifier found it really hard to generate a good decision region, am I a hard user to please?**

