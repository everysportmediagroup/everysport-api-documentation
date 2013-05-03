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

## Sport object format
Represents a sport.

Includes the following data:
* id - the sport ID, integer
* name - the full name of the sport, string


## League object format
Represents a league, regardless of sport.

Includes the following data:
* id - a unique league  id, integer
* name - the full name of the league, string
* teamClass - one of 'men','women','mixed'
* sport - a Sport object

## Team object format
Represents a team, regardless of sport.

### Team short format
* id - the team ID, integer
* name - the full name of the team, string
* shortName - a shorter version of the name, string
* abbreviation - an abbreviated form of the name, string
* link - a URL to the team's page at everysport.com, url string

## Player object format 
Represents a player

### Player short format
* name - Name of the player

## Event object format
A generic object that may represent a game/match regardless of sport. 

### Event short format
* id - a unique event id, integer
* status - one of 'upcoming','ongoing','finished', 'postponed', 'interrupted'
* startDate - scheduled start date of the event, Date long format
* visitingTeamScore - score of visiting team, integer or null
* homeTeamScore - score of home team, integer or null
* visitingTeam - a Team object in small format
* homeTeam - a Team object in small format
* round - the round in which the game belongs, integer or null 

### Extended format
* facts - Details information such as spectators, arena and referees
* gameEventLevel - The level of detail that the game event list contains, 'detailed' or 'aggregated'
* gameEvents - Game events for this event, Array of GameEvent objects
* subGames - Sub games for this event, Array of SubGame objects

## GameEvent object format
Events from a game, for example goals, penalties and period results.
Each type of game event have its own set of properties.

### All game events:
* type - Type of game event

### Game events of type 'PERIOD_RESULT'
* period - what period the result refers to, integer
* homeTeamPeriodScore - how many goals the home team scored in the period, integer
* visitingTeamPeriodScore - how many goals the visiting team scored in the period, integer

### Game events of type 'ORDINARY_TIME_RESULT'
* homeTeamScore - Score for the home team after the ordinary number of periods has been played, integer
* visitingTeamScore - Score for the visiting team after the ordinary number of periods has been played, integer

### Game events of type 'GOAL'
* minute - Game minute the goal was made, only present if the game event level is detailed, integer
* second - Game second the goal was made, only present if the game event level is detailed, integer
* count - Number of goals accounted for this game event, always 1 when the game event level is detailed, integer
* penaltyShot - Number of goals made from a penalty shot of the total count for the game event, 0 or 1 when the game event level is detailed, integer
* team - The team that scored the goal, a Team object in small format
* player - The player that scored the goal, a Player object in small format
* assistingPlayers - The players that assisted the goal, Array of Player objects in small format
* homeTeamScore - Score for the home team after the goal, only present if the game event level is detailed, integer
* visitingTeamScore - Score for the visiting team after the goal, only present if the game event level is detailed, integer

## SubGame object format
Some events consists of many games that are represented as sub games. This is common in Tennis and Table tennis.

### Format
* gameNumber - Number for this game in the serie of sub games
* visitingTeam - a Team object in small format
* homeTeam - a Team object in small format
* visitingTeamPlayer - optional, a Player object in small format
* homeTeamPlayer - optional, a Player object in small format
* scores - Period scores from the game for both teams, Array of objects with homeTeamScore and visitingTeamScore properties. 

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
