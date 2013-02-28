# Formats and Terms
Here are the generic formats and terms used in the API. 

## League ID
To find the League ID, look up the league at [everysport.com](http://www.everysport.com). The ID is the last digits in the URL. 

http://www.everysport.com/sport/ishockey/2012-2013/elitserien-herr/elitserien/54258

Note that the League ID is different for each season. The League ID is 54258 for the swedish hockey league “Elitserien” in 2012-13.

## Dates
Dates are used in several places, in short and long format.

### Date short format
Dates in short format are YYYY-MM-DD

### Date long format
Dates in long format are according to [ISO 8601](http://en.wikipedia.org/wiki/ISO_8601) format


## Credits objects
Almost every return value contains a standard Credits object. It contains the necessary information to display with the data, as defined in [API Terms of Use](/basics/terms_of_use.md) to give Everysport credit for providing the data. 

### Credits format
* message - "Provided by Everysport.com", string
* link - a URL link to relevant part of everysport.com, url string
* logoUrl - the Everysport logo, url string

## Team object format
Represents a team, regardless of sport.

### Team short format
* id - the team ID, integer
* name - the full name of the team, string
* shortName - a shorter version of the name, string
* abbreviation - an abbreviated form of the name, string
* link - a URL to the team's page at everysport.com, url string

## Event object format
A generic object that may represent a game/match regardless of sport. 

Includes the following data:
* id - a unique event id, integer
* status - one of 'upcoming','ongoing','finished', 'postponed', 'interrupted', 'all'(default)
* startDate - scheduled start date of the event, Date long format
* visitingTeamScore - score of visiting team, integer or null
* homeTeamScore - score of home team, integer or null
* visitingTeam - a Team object in small format
* homeTeam - a Team object in small format
* round - the round in which the game belongs, integer or null 

## Team Stats object format
Used to represent the results and stats for the team, for example, currently in the league table.  

Different teams use different sets of stats data. For example, while most leagues have Won, Loss and Draws, some leagues also have Overtime Loss and Overtime Won. 
The calculation of total points is also league-dependent. 

The Stats objects may include (league-dependant) the following data:
* gp - games played, integer
* w - won, integer
* d - draws, integer
* l - loss, integer
* ol - overtime loss, integer
* ow - overtime won, integer
* gf - goals forward, integer
* ga - goals against, integer
* gd - goals differential, integer
* pts - points, integer

Note that gp = w + d + l + ol + ow and that gd = gf - ga.
