# Standings

    GET leagues/:id/standings

## Description
Returns a list of the current standings (i.e. the tables) for the league. 

A league may contain one or many groups. For example, the NHL league has several groups, such as the conferences (Eastern and Western) and divisions (Atlantic, Pacific, etc.). One team may belong to more than one group. Most leagues, however, has only one group. 

The league standings, commonly visualized as a table, is essentially a list of the teams and their respective stats, sorted by one of the stats attributes, normally the total points. 

## Parameters
* id (required) - The League ID
* apikey (required) - your APIKEY
* type - one of 'total' (default), 'home' and 'away' 
* size - specifies the amount of statistics data for the teams. Default is 'large' which retrieves all available data. Use  'medium' and 'small' to get less data. 
* sortKey - the key by which the standings is sorted. Can be any of the attribute names from the Team Stats objects (eg. 'stats.pts') or 'team.name' to sort by the name of the team. By default, sorting is by 'stats.pts'.   
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 


## Example Request

GET /leagues/58878/standings

```javascript	
{
credit: {
message: "Provided by Everysport.com",
link: "http://www.everysport.com",
logoUrl: "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png"
},
groups: [
{
labels: [
{
type: "conference",
name: "Western Conference"
},
{
type: "division",
name: "Central Division"
}
],
standings: [
{
team: {
id: 28075,
name: "Chicago Blackhawks",
shortName: "Chicago",
link: "http://www.everysport.com/sport/ishockey/team/chicago-blackhawks/28075"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 16
},
{
name: "l",
value: 0
},
{
name: "gf",
value: 61
},
{
name: "ga",
value: 37
},
{
name: "gd",
value: 24
},
{
name: "pts",
value: 35
}
]
},
{
team: {
id: 28067,
name: "Nashville Predators",
shortName: "Nashville",
link: "http://www.everysport.com/sport/ishockey/team/nashville-predators/28067"
},
stats: [
{
name: "gp",
value: 21
},
{
name: "w",
value: 9
},
{
name: "l",
value: 7
},
{
name: "gf",
value: 45
},
{
name: "ga",
value: 52
},
{
name: "gd",
value: -7
},
{
name: "pts",
value: 23
}
]
},
{
team: {
id: 28072,
name: "St Louis Blues",
shortName: "St Louis",
link: "http://www.everysport.com/sport/ishockey/team/st-louis-blues/28072"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 10
},
{
name: "l",
value: 6
},
{
name: "gf",
value: 55
},
{
name: "ga",
value: 52
},
{
name: "gd",
value: 3
},
{
name: "pts",
value: 22
}
]
},
{
team: {
id: 28071,
name: "Detroit Red Wings",
shortName: "Detroit",
link: "http://www.everysport.com/sport/ishockey/team/detroit-red-wings/28071"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 9
},
{
name: "l",
value: 8
},
{
name: "gf",
value: 58
},
{
name: "ga",
value: 56
},
{
name: "gd",
value: 2
},
{
name: "pts",
value: 21
}
]
},
{
team: {
id: 28074,
name: "Columbus Blue Jackets",
shortName: "Columbus",
link: "http://www.everysport.com/sport/ishockey/team/columbus-blue-jackets/28074"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 5
},
{
name: "l",
value: 12
},
{
name: "gf",
value: 44
},
{
name: "ga",
value: 61
},
{
name: "gd",
value: -17
},
{
name: "pts",
value: 13
}
]
}
]
},
{
labels: [
{
type: "conference",
name: "Western Conference"
},
{
type: "division",
name: "Northwest Division"
}
],
standings: [
{
team: {
id: 28063,
name: "Vancouver Canucks",
shortName: "Vancouver",
link: "http://www.everysport.com/sport/ishockey/team/vancouver-canucks/28063"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 10
},
{
name: "l",
value: 5
},
{
name: "gf",
value: 54
},
{
name: "ga",
value: 52
},
{
name: "gd",
value: 2
},
{
name: "pts",
value: 24
}
]
},
{
team: {
id: 28057,
name: "Minnesota Wild",
shortName: "Minnesota",
link: "http://www.everysport.com/sport/ishockey/team/minnesota-wild/28057"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 9
},
{
name: "l",
value: 7
},
{
name: "gf",
value: 39
},
{
name: "ga",
value: 43
},
{
name: "gd",
value: -4
},
{
name: "pts",
value: 20
}
]
},
{
team: {
id: 28053,
name: "Edmonton Oilers",
shortName: "Edmonton",
link: "http://www.everysport.com/sport/ishockey/team/edmonton-oilers/28053"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 7
},
{
name: "l",
value: 7
},
{
name: "gf",
value: 42
},
{
name: "ga",
value: 49
},
{
name: "gd",
value: -7
},
{
name: "pts",
value: 18
}
]
},
{
team: {
id: 28058,
name: "Calgary Flames",
shortName: "Calgary",
link: "http://www.everysport.com/sport/ishockey/team/calgary-flames/28058"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 7
},
{
name: "l",
value: 7
},
{
name: "gf",
value: 49
},
{
name: "ga",
value: 61
},
{
name: "gd",
value: -12
},
{
name: "pts",
value: 18
}
]
},
{
team: {
id: 28054,
name: "Colorado Avalanche",
shortName: "Colorado",
link: "http://www.everysport.com/sport/ishockey/team/colorado-avalanche/28054"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 7
},
{
name: "l",
value: 8
},
{
name: "gf",
value: 44
},
{
name: "ga",
value: 54
},
{
name: "gd",
value: -10
},
{
name: "pts",
value: 17
}
]
}
]
},
{
labels: [
{
type: "conference",
name: "Western Conference"
},
{
type: "division",
name: "Pacific Division"
}
],
standings: [
{
team: {
id: 28076,
name: "Anaheim Ducks",
shortName: "Anaheim",
link: "http://www.everysport.com/sport/ishockey/team/anaheim-ducks/28076"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 14
},
{
name: "l",
value: 3
},
{
name: "gf",
value: 64
},
{
name: "ga",
value: 48
},
{
name: "gd",
value: 16
},
{
name: "pts",
value: 29
}
]
},
{
team: {
id: 28060,
name: "Los Angeles Kings",
shortName: "Los Angeles",
link: "http://www.everysport.com/sport/ishockey/team/los-angeles-kings/28060"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 10
},
{
name: "l",
value: 6
},
{
name: "gf",
value: 47
},
{
name: "ga",
value: 42
},
{
name: "gd",
value: 5
},
{
name: "pts",
value: 22
}
]
},
{
team: {
id: 28059,
name: "Dallas Stars",
shortName: "Dallas",
link: "http://www.everysport.com/sport/ishockey/team/dallas-stars/28059"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 10
},
{
name: "l",
value: 8
},
{
name: "gf",
value: 56
},
{
name: "ga",
value: 57
},
{
name: "gd",
value: -1
},
{
name: "pts",
value: 22
}
]
},
{
team: {
id: 28064,
name: "Phoenix Coyotes",
shortName: "Phoenix",
link: "http://www.everysport.com/sport/ishockey/team/phoenix-coyotes/28064"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 9
},
{
name: "l",
value: 7
},
{
name: "gf",
value: 54
},
{
name: "ga",
value: 51
},
{
name: "gd",
value: 3
},
{
name: "pts",
value: 21
}
]
},
{
team: {
id: 28068,
name: "San Jose Sharks",
shortName: "San Jose",
link: "http://www.everysport.com/sport/ishockey/team/san-jose-sharks/28068"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 9
},
{
name: "l",
value: 6
},
{
name: "gf",
value: 44
},
{
name: "ga",
value: 41
},
{
name: "gd",
value: 3
},
{
name: "pts",
value: 21
}
]
}
]
},
{
labels: [
{
type: "conference",
name: "Eastern Conference"
},
{
type: "division",
name: "Atlantic Division"
}
],
standings: [
{
team: {
id: 28062,
name: "Pittsburgh Penguins",
shortName: "Pittsburgh",
link: "http://www.everysport.com/sport/ishockey/team/pittsburgh-penguins/28062"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 13
},
{
name: "l",
value: 7
},
{
name: "gf",
value: 69
},
{
name: "ga",
value: 54
},
{
name: "gd",
value: 15
},
{
name: "pts",
value: 26
}
]
},
{
team: {
id: 28061,
name: "New Jersey Devils",
shortName: "New Jersey",
link: "http://www.everysport.com/sport/ishockey/team/new-jersey-devils/28061"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 10
},
{
name: "l",
value: 5
},
{
name: "gf",
value: 48
},
{
name: "ga",
value: 49
},
{
name: "gd",
value: -1
},
{
name: "pts",
value: 24
}
]
},
{
team: {
id: 28069,
name: "Philadelphia Flyers",
shortName: "Philadelphia",
link: "http://www.everysport.com/sport/ishockey/team/philadelphia-flyers/28069"
},
stats: [
{
name: "gp",
value: 22
},
{
name: "w",
value: 10
},
{
name: "l",
value: 11
},
{
name: "gf",
value: 64
},
{
name: "ga",
value: 67
},
{
name: "gd",
value: -3
},
{
name: "pts",
value: 21
}
]
},
{
team: {
id: 28070,
name: "New York Rangers",
shortName: "NY Rangers",
link: "http://www.everysport.com/sport/ishockey/team/new-york-rangers/28070"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 8
},
{
name: "l",
value: 8
},
{
name: "gf",
value: 44
},
{
name: "ga",
value: 48
},
{
name: "gd",
value: -4
},
{
name: "pts",
value: 18
}
]
},
{
team: {
id: 28052,
name: "New York Islanders",
shortName: "NY Islanders",
link: "http://www.everysport.com/sport/ishockey/team/new-york-islanders/28052"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 8
},
{
name: "l",
value: 11
},
{
name: "gf",
value: 57
},
{
name: "ga",
value: 68
},
{
name: "gd",
value: -11
},
{
name: "pts",
value: 17
}
]
}
]
},
{
labels: [
{
type: "conference",
name: "Eastern Conference"
},
{
type: "division",
name: "Northeast Division"
}
],
standings: [
{
team: {
id: 28066,
name: "Montreal Canadiens",
shortName: "Montreal",
link: "http://www.everysport.com/sport/ishockey/team/montreal-canadiens/28066"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 13
},
{
name: "l",
value: 4
},
{
name: "gf",
value: 58
},
{
name: "ga",
value: 43
},
{
name: "gd",
value: 15
},
{
name: "pts",
value: 29
}
]
},
{
team: {
id: 28065,
name: "Boston Bruins",
shortName: "Boston",
link: "http://www.everysport.com/sport/ishockey/team/boston-bruins/28065"
},
stats: [
{
name: "gp",
value: 16
},
{
name: "w",
value: 12
},
{
name: "l",
value: 2
},
{
name: "gf",
value: 49
},
{
name: "ga",
value: 35
},
{
name: "gd",
value: 14
},
{
name: "pts",
value: 26
}
]
},
{
team: {
id: 28050,
name: "Ottawa Senators",
shortName: "Ottawa",
link: "http://www.everysport.com/sport/ishockey/team/ottawa-senators/28050"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 12
},
{
name: "l",
value: 6
},
{
name: "gf",
value: 48
},
{
name: "ga",
value: 37
},
{
name: "gd",
value: 11
},
{
name: "pts",
value: 26
}
]
},
{
team: {
id: 28049,
name: "Toronto Maple Leafs",
shortName: "Toronto",
link: "http://www.everysport.com/sport/ishockey/team/toronto-maple-leafs/28049"
},
stats: [
{
name: "gp",
value: 21
},
{
name: "w",
value: 12
},
{
name: "l",
value: 9
},
{
name: "gf",
value: 59
},
{
name: "ga",
value: 51
},
{
name: "gd",
value: 8
},
{
name: "pts",
value: 24
}
]
},
{
team: {
id: 28051,
name: "Buffalo Sabres",
shortName: "Buffalo",
link: "http://www.everysport.com/sport/ishockey/team/buffalo-sabres/28051"
},
stats: [
{
name: "gp",
value: 20
},
{
name: "w",
value: 7
},
{
name: "l",
value: 12
},
{
name: "gf",
value: 50
},
{
name: "ga",
value: 64
},
{
name: "gd",
value: -14
},
{
name: "pts",
value: 15
}
]
}
]
},
{
labels: [
{
type: "conference",
name: "Eastern Conference"
},
{
type: "division",
name: "Southeast Division"
}
],
standings: [
{
team: {
id: 28055,
name: "Tampa Bay Lightning",
shortName: "Tampa Bay",
link: "http://www.everysport.com/sport/ishockey/team/tampa-bay-lightning/28055"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 9
},
{
name: "l",
value: 9
},
{
name: "gf",
value: 70
},
{
name: "ga",
value: 60
},
{
name: "gd",
value: 10
},
{
name: "pts",
value: 19
}
]
},
{
team: {
id: 28056,
name: "Carolina Hurricanes",
shortName: "Carolina",
link: "http://www.everysport.com/sport/ishockey/team/carolina-hurricanes/28056"
},
stats: [
{
name: "gp",
value: 18
},
{
name: "w",
value: 9
},
{
name: "l",
value: 8
},
{
name: "gf",
value: 50
},
{
name: "ga",
value: 54
},
{
name: "gd",
value: -4
},
{
name: "pts",
value: 19
}
]
},
{
team: {
id: 109005,
name: "Winnipeg Jets",
shortName: "Winnipeg",
link: "http://www.everysport.com/sport/ishockey/team/winnipeg-jets/109005"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 9
},
{
name: "l",
value: 9
},
{
name: "gf",
value: 52
},
{
name: "ga",
value: 60
},
{
name: "gd",
value: -8
},
{
name: "pts",
value: 19
}
]
},
{
team: {
id: 28047,
name: "Florida Panthers",
shortName: "Florida",
link: "http://www.everysport.com/sport/ishockey/team/florida-panthers/28047"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 6
},
{
name: "l",
value: 9
},
{
name: "gf",
value: 48
},
{
name: "ga",
value: 69
},
{
name: "gd",
value: -21
},
{
name: "pts",
value: 16
}
]
},
{
team: {
id: 28073,
name: "Washington Capitals",
shortName: "Washington",
link: "http://www.everysport.com/sport/ishockey/team/washington-capitals/28073"
},
stats: [
{
name: "gp",
value: 19
},
{
name: "w",
value: 7
},
{
name: "l",
value: 11
},
{
name: "gf",
value: 52
},
{
name: "ga",
value: 59
},
{
name: "gd",
value: -7
},
{
name: "pts",
value: 15
}
]
}
]
}
]
}
```


	
        	
