Bookworm sentiment analysis
===========================


This is a placeholder for some scripts that will add the results of sentiment analysis into a Bookworm browser.

The basic inspiration, and the sources for sentiment analysis packages, come from [Matt Jockers Syuzhet package](https://github.com/mjockers/syuzhet). 


Currently this includes one list: the NRC list of emotions from here.

> Saif Mohammad and Peter Turney.  "Emotions Evoked by Common Words and Phrases: Using Mechanical Turk to Create an Emotion Lexicon." In Proceedings of the NAACL-HLT 2010 Workshop on Computational Approaches to Analysis and Generation of Emotion in Text, June 2010, LA, California.  See: http://saifmohammad.com/WebPages/lexicons.html

This will ultimately load that in and tag each text by its ratio on each of those scores, somehow.

It should also allow parsing with the Stanford Sentiment tagger: the current problem is that it isn't immediately obvious how to massively parallelize that, since it outputs a sentiment for each sentence, but the overhead for launching the scanner once per file is probably prohibitive on hundreds of thousands of files.
