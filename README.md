# How to make your own "Musikquiz"

I like using the popular Danish radioshow "Musikquizzen" as a basis for a quick quiz with friends. These are the steps I take to cut a single quiz.

This is mainly a document for myself, as I keep forgetting the (very simple) steps.

## Steps
### Find the relevant episode
For this example we know that we want to make a quiz from the show aired 2022-01-23, starting from about 1h12 into the show. 

### Download the episode
The show homepage is here: https://www.dr.dk/lyd/p4/musikquizzen/
The RSS feed is here: https://www.dr.dk/mu/feed/musikquizzen.xml?format=podcast

Download the RSS feed and search for the URL of the relevant episode. In this case, I found it by searching for "2022-01-23". 

Download the episode
```
wget https://www.dr.dk/mu/MediaRedirector/WithFileExtension/musikquizzen-2022-01-23.mp3\?highestBitrate\=True\&amp\;podcastDownload\=True -o musikquiz.mp3
```

### Edit the episode
I'm using Audacity to cut up the relevant parts of the episode. It's available in the Ubuntu Software Store.

1) Import the mp3 file to make a new project.
2) Go to the start of the relevant part, start listening. Start taking notes on 
   - Timestamps for start and end
   - Questions and correct answers
3) Mark the start and end of the quiz and copy it to a new track. Delete the old tracks and "Fit project to width (Ctrl+F)". Now it should be easier to see silences and that makes cutting easier.
4) Listen again and start copying the questions and answers to a new track.

Tips:
- You can give a name to each soundbite. This makes it easier to have an overview of the process.
- When you have collected all the clips, you need to but in a pause between each Question and Answer. I like to put in about 5 seconds between each clip.
- If you start spacing out clips from the last clip, it makes it easy to have enough "room" for all of them.