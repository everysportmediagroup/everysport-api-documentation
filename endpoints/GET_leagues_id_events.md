# Events

    GET leagues/:id/events

## Description
Returns a list of Event objects for the league.

## Resource URL

		http://api.everysport.com/v1/leagues/:id/events


## Parameters
* id (required) - the League ID
* apikey (required) - your APIKEY
* status - a comma-seperated list of one or many status, for which you want to filter the events. Can be any status value as defined by the Event object.
* fromDate - filters out events after a specific date, Date in short format
* toDate - filters out events before a specific date, Date in short format
* round - a comma-seperated list of one or many rounds, for which you want to filter the events.
* limit - Limits the number of events, positive integer
* offset - Indicates where to start in the list. Defaults to 0, positive integer
* sort - the property and order by which the events is sorted. Can be 'startDate:asc', 'startDate:desc', 'round:asc' or 'round:desc'. Default is 'startDate:asc'.
* team - a comma-separated list of one or many team IDs, for which you want to filter the events.  
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esEvents'


## Example Request
```
GET http://api.everysport.com/v1/leagues/58878/events?limit=10&status=upcoming
```

```javascript
{
credit: {
message: "Provided by Everysport.com",
link: "http://www.everysport.com",
logoUrl: "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png"
},
metadata: {
limit: 10,
count: 10,
totalCount: 713,
offset: 0
},
events: [
{
id: 2135253,
startDate: "2013-01-19T01:00+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28069,
shortName: "Philadelphia",
link: "http://www.everysport.com/sport/ishockey/team/philadelphia/28069"
},
visitingTeam: {
id: 28062,
shortName: "Pittsburgh",
link: "http://www.everysport.com/sport/ishockey/team/pittsburgh/28062"
},
homeTeamScore: 1,
visitingTeamScore: 3,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135257,
startDate: "2013-01-19T01:00+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28066,
shortName: "Montreal",
link: "http://www.everysport.com/sport/ishockey/team/montreal/28066"
},
visitingTeam: {
id: 28049,
shortName: "Toronto",
link: "http://www.everysport.com/sport/ishockey/team/toronto/28049"
},
homeTeamScore: 1,
visitingTeamScore: 2,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135258,
startDate: "2013-01-19T01:00+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28052,
shortName: "NY Islanders",
link: "http://www.everysport.com/sport/ishockey/team/ny-islanders/28052"
},
visitingTeam: {
id: 28061,
shortName: "New Jersey",
link: "http://www.everysport.com/sport/ishockey/team/new-jersey/28061"
},
homeTeamScore: 1,
visitingTeamScore: 2,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135256,
startDate: "2013-01-19T01:30+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28065,
shortName: "Boston",
link: "http://www.everysport.com/sport/ishockey/team/boston/28065"
},
visitingTeam: {
id: 28070,
shortName: "NY Rangers",
link: "http://www.everysport.com/sport/ishockey/team/ny-rangers/28070"
},
homeTeamScore: 3,
visitingTeamScore: 1,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135259,
startDate: "2013-01-19T01:30+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28055,
shortName: "Tampa Bay",
link: "http://www.everysport.com/sport/ishockey/team/tampa-bay/28055"
},
visitingTeam: {
id: 28073,
shortName: "Washington",
link: "http://www.everysport.com/sport/ishockey/team/washington/28073"
},
homeTeamScore: 6,
visitingTeamScore: 3,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135260,
startDate: "2013-01-19T01:30+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28047,
shortName: "Florida",
link: "http://www.everysport.com/sport/ishockey/team/florida/28047"
},
visitingTeam: {
id: 28056,
shortName: "Carolina",
link: "http://www.everysport.com/sport/ishockey/team/carolina/28056"
},
homeTeamScore: 5,
visitingTeamScore: 1,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135264,
startDate: "2013-01-19T02:00+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28057,
shortName: "Minnesota",
link: "http://www.everysport.com/sport/ishockey/team/minnesota/28057"
},
visitingTeam: {
id: 28054,
shortName: "Colorado",
link: "http://www.everysport.com/sport/ishockey/team/colorado/28054"
},
homeTeamScore: 4,
visitingTeamScore: 2,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135263,
startDate: "2013-01-19T02:30+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28059,
shortName: "Dallas",
link: "http://www.everysport.com/sport/ishockey/team/dallas/28059"
},
visitingTeam: {
id: 28064,
shortName: "Phoenix",
link: "http://www.everysport.com/sport/ishockey/team/phoenix/28064"
},
homeTeamScore: 4,
visitingTeamScore: 3,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2135262,
startDate: "2013-01-19T03:00+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28067,
shortName: "Nashville",
link: "http://www.everysport.com/sport/ishockey/team/nashville/28067"
},
visitingTeam: {
id: 28074,
shortName: "Columbus",
link: "http://www.everysport.com/sport/ishockey/team/columbus/28074"
},
homeTeamScore: 2,
visitingTeamScore: 3,
finishedTimeStatus: "PENALTY_SHOOTOUT"
},
{
id: 2135267,
startDate: "2013-01-19T03:30+01",
round: 1,
status: "FINISHED",
homeTeam: {
id: 28058,
shortName: "Calgary",
link: "http://www.everysport.com/sport/ishockey/team/calgary/28058"
},
visitingTeam: {
id: 28068,
shortName: "San Jose",
link: "http://www.everysport.com/sport/ishockey/team/san-jose/28068"
},
homeTeamScore: 1,
visitingTeamScore: 4,
finishedTimeStatus: "ORDINARY_TIME"
}
]
}
```
