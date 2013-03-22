# Norsk Sentiment Analayse #

Et lite eksperiment med norsk sentimentanalyse i Ruby. Start programmet fra
kommandolinjen, tast inn et ord og vent på at programmet søker etter ordet
på twitter og returnerer antall positive og negative tweets.

    $ ruby tweet-search-sentiment.rb
    Enter search term: påske
    Accessing tweets using search term: påske...
    http://search.twitter.com/search.json?q=p%C3%A5ske&rpp=100&page=1
    http://search.twitter.com/search.json?q=p%C3%A5ske&rpp=100&page=2
    http://search.twitter.com/search.json?q=p%C3%A5ske&rpp=100&page=3
    ...
    Number of tweets analyzed: 1000
    Negative tweets: 52
    Neutral tweets: 770
    Positive tweets: 178
    Search term "påske" had a 77% positive sentiment.

# Sentiment analyse #

Sentiment analyse er basert på en ordliste på 1561 ord, hvor hvert ord har en
score mellom +4 og -4 avhengig av om ordet er positivt eller negativt.

Ordlisten er oversatt fra dansk, og forhåpentligvis basert på en analyse av språket.

# Credits

  Original author Chris MacLellan
