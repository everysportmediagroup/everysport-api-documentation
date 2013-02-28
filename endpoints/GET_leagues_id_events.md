# Events

    GET leagues/:id/events

## Description
Returns a list of Event objects for the league.

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
GET /leagues/58878/events?limit=10&status=upcoming
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
totalCount: 427,
offset: 0
},
events: [
{
id: 2136405,
startDate: "2013-03-01T01:00+01",
round: 19,
status: "UPCOMING",
homeTeam: {
id: 28065,
shortName: "Boston",
link: "http://www.everysport.com/sport/ishockey/team/null/28065"
},
visitingTeam: {
id: 28050,
shortName: "Ottawa",
link: "http://www.everysport.com/sport/ishockey/team/null/28050"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136406,
startDate: "2013-03-01T01:00+01",
round: 19,
status: "UPCOMING",
homeTeam: {
id: 28052,
shortName: "NY Islanders",
link: "http://www.everysport.com/sport/ishockey/team/null/28052"
},
visitingTeam: {
id: 28049,
shortName: "Toronto",
link: "http://www.everysport.com/sport/ishockey/team/null/28049"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136407,
startDate: "2013-03-01T01:00+01",
round: 19,
status: "UPCOMING",
homeTeam: {
id: 28070,
shortName: "NY Rangers",
link: "http://www.everysport.com/sport/ishockey/team/null/28070"
},
visitingTeam: {
id: 28055,
shortName: "Tampa Bay",
link: "http://www.everysport.com/sport/ishockey/team/null/28055"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136408,
startDate: "2013-03-01T01:00+01",
round: 19,
status: "UPCOMING",
homeTeam: {
id: 28056,
shortName: "Carolina",
link: "http://www.everysport.com/sport/ishockey/team/null/28056"
},
visitingTeam: {
id: 28062,
shortName: "Pittsburgh",
link: "http://www.everysport.com/sport/ishockey/team/null/28062"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136409,
startDate: "2013-03-01T01:30+01",
round: 19,
status: "UPCOMING",
homeTeam: {
id: 28047,
shortName: "Florida",
link: "http://www.everysport.com/sport/ishockey/team/null/28047"
},
visitingTeam: {
id: 28051,
shortName: "Buffalo",
link: "http://www.everysport.com/sport/ishockey/team/null/28051"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136410,
startDate: "2013-03-01T02:00+01",
round: 19,
status: "UPCOMING",
homeTeam: {
id: 109005,
shortName: "Winnipeg",
link: "http://www.everysport.com/sport/ishockey/team/null/109005"
},
visitingTeam: {
id: 28061,
shortName: "New Jersey",
link: "http://www.everysport.com/sport/ishockey/team/null/28061"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136411,
startDate: "2013-03-01T02:00+01",
round: 20,
status: "UPCOMING",
homeTeam: {
id: 28072,
shortName: "St Louis",
link: "http://www.everysport.com/sport/ishockey/team/null/28072"
},
visitingTeam: {
id: 28075,
shortName: "Chicago",
link: "http://www.everysport.com/sport/ishockey/team/null/28075"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136412,
startDate: "2013-03-01T02:30+01",
round: 20,
status: "UPCOMING",
homeTeam: {
id: 28059,
shortName: "Dallas",
link: "http://www.everysport.com/sport/ishockey/team/null/28059"
},
visitingTeam: {
id: 28053,
shortName: "Edmonton",
link: "http://www.everysport.com/sport/ishockey/team/null/28053"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136413,
startDate: "2013-03-01T03:00+01",
round: 20,
status: "UPCOMING",
homeTeam: {
id: 28054,
shortName: "Colorado",
link: "http://www.everysport.com/sport/ishockey/team/null/28054"
},
visitingTeam: {
id: 28058,
shortName: "Calgary",
link: "http://www.everysport.com/sport/ishockey/team/null/28058"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
},
{
id: 2136414,
startDate: "2013-03-01T03:00+01",
round: 20,
status: "UPCOMING",
homeTeam: {
id: 28064,
shortName: "Phoenix",
link: "http://www.everysport.com/sport/ishockey/team/null/28064"
},
visitingTeam: {
id: 28057,
shortName: "Minnesota",
link: "http://www.everysport.com/sport/ishockey/team/null/28057"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME"
}
]
}
```
