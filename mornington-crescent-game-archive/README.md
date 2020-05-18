# Mornington Crescent Game Archive

> Visit my [Blog](http://www.rai.org.uk) to get in touch or to see demos of my other work.

## Overview

Welcome to this archive! _You've found the Wisden of Mornington Crescent._

Here you will find a detailed record of _every single game of Mornington Crescent that has ever been played_, since its inception in late August 1978 to the start of 2020. The archive scope is all games played in tournaments, leagues, clubs and societies. This is pretty much the whole shebang for the game history - barring personal games, pub games and things like random games played on [radio shows](https://en.wikipedia.org/wiki/I%27m_Sorry_I_Haven%27t_a_Clue) and such.

> If you don't care about all the details and just want to explore the data, then you can use the [Game Explorer](https://pete-rai.github.io/mornington-crescent-game-archive/) site for that.

## The Opportunity

This is a huge opportunity for any machine learning experts. I know that, in the past, ML researchers have balked at the complexity of taking on Mornington Crescent and have instead taken on simpler games such as [Chess](https://en.wikipedia.org/wiki/Deep_Blue_(chess_computer)) and [Go](https://en.wikipedia.org/wiki/AlphaGo). But now the data exists in one place and one format, I hope that teams will step-up and try and build the first ever, credible robot player of this _very human_ game.

## The Corpus

Gathering this collection has been a labour of love for more than a decade. The records are quite literally 'all over the place'. A key achievement was that I was granted (after a great deal of wrangling) access to the Knoeppfler archives. My sincere thanks to Dr Knoeppfler's family for allowing me to consult this tremendous resource. The Knoeppfler records were hand written in tiny German script and I was not allowed (for obvious reasons) to remove the paper records from the estate - so this was a huge and time consuming challenge.

I have included all the major game playing organisations worldwide. An odd-ball being the Indian Leagues, which disbanded in late 1998 (after fallout from the Fairlop schism). However, luckily in 2004 records of these were found in a locked cabinet in a basement of Mumbai's [Chunabhatti station](https://en.wikipedia.org/wiki/Chunabhatti_railway_station).

I have _not_ included games played under 'Finchley Central' rules. This should not be a surprise, as this is _not_ Mornington Crescent - it is a totally different game! The 'Finchley Central' players are a strange bunch indeed, but as true aficionados of the game know, FC is not cannon. Also, please don't get me started on The Hornchurch Convention weirdos. I will leave it to our American cousins to digitise the Grand Central games.

## The Data

All the data is in the one file [games.json]() and, as the name suggests, is held in JSON format. It is giant array consisting of over 18,000 items. Each item is a single game in the following format:

```json
{
    "id": "707dcb38558c343d10c97b8f",
    "started": "1978-09-22",
    "duration": 114,
    "players": 2,
    "winner": 2,
    "tags": [
        "Laterals disallowed",
        "Interchanges disallowed",
        "Loops inverted"
    ],
    "moves": [
        {
            "player": 1,
            "move": "Kentish Town",
            "note": ""
        },
        {
            "player": 2,
            "move": "Saint Pauls",
            "note": "opponent denied left"
        },
        {
            "player": 1,
            "move": "Westminster",
            "note": "challenge | rejected | Loops inverted"
        },
        {
            "player": 2,
            "move": "Newbury Park",
            "note": ""
        },
        {
            "player": 1,
            "move": "Tower Hill",
            "note": "on the reverse"
        },
        {
            "player": 2,
            "move": "Mornington Crescent",
            "note": ""
        }
    ]
},
```

Note that "id" is always a 28 character string, "started" dates are always in the format YYYY-MM-DD and "duration" is always measured in seconds.

Happy Mornington Crescent playing and watch-this-space for the upcoming _Wobbling Bunnies_ game archive.

_– [Pete Rai](http://www.rai.org.uk)_
