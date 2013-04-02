# Events

    GET events

## Description
Returns a list of Event objects.  

## Parameters
* id (required) - the League ID
* apikey (required) - your APIKEY
* league - a comma-separated list of league IDs, for which to retrieve events.
* status - a comma-seperated list of one or many status, for which to retrieve events. Can be any status value as defined by the Event object.
* fromDate - filters out events after a specific date, Date in short format
* toDate - filters out events before a specific date, Date in short format
* round - a comma-seperated list of one or many rounds, for which to retrieve events.
* limit - Limits the number of events, positive integer
* offset - Indicates where to start in the list. Defaults to 0, positive integer
* sort - the property and order by which the events is sorted. Can be 'startDate:asc', 'startDate:desc', 'round:asc' or 'round:desc'. Default is 'startDate:asc'.
* team - a comma-separated list of one or many team IDs, for which to retrieve events.  
* sport - a comma-separated list of one or many sport IDs, for which to retrieve events.  
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esEvents'

## Return format

```javascript	
{
	credit: {
	message: "Provided by Everysport.com",
	link: "http://www.everysport.com",
	logoUrl: "http://c.static.es-cdn.net/files/everysport2/images/	icons/event/small/everysport.png"
},
	metadata: {
	limit: 3,
	count: 3,
	totalCount: 914,
	offset: 0
},
events: [
{
id: 2044519,
startDate: "2012-08-18T15:00+0200",
round: 1,
status: "FINISHED",
homeTeam: {
id: 27681,
name: "Arsenal",
shortName: "Arsenal",
link: "http://www.everysport.com/sport/fotboll/team/arsenal/27681"
},
visitingTeam: {
id: 27669,
name: "Sunderland",
shortName: "Sunderland",
link: "http://www.everysport.com/sport/fotboll/team/sunderland/27669"
},
homeTeamScore: 0,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME",
league: {
id: 55193,
name: "Premier League"
}
},
{
id: 2044520,
startDate: "2012-08-18T15:00+0200",
round: 1,
status: "FINISHED",
homeTeam: {
id: 27675,
name: "Fulham",
shortName: "Fulham",
link: "http://www.everysport.com/sport/fotboll/team/fulham/27675"
},
visitingTeam: {
id: 27703,
name: "Norwich",
shortName: "Norwich",
link: "http://www.everysport.com/sport/fotboll/team/norwich/27703"
},
homeTeamScore: 5,
visitingTeamScore: 0,
finishedTimeStatus: "ORDINARY_TIME",
league: {
id: 55193,
name: "Premier League"
}
},
{
id: 2044521,
startDate: "2012-08-18T15:00+0200",
round: 1,
status: "FINISHED",
homeTeam: {
id: 27694,
name: "Queens PR",
shortName: "QPR",
link: "http://www.everysport.com/sport/fotboll/team/queens-pr/27694"
},
visitingTeam: {
id: 27711,
name: "Swansea",
shortName: "Swansea",
link: "http://www.everysport.com/sport/fotboll/team/swansea/27711"
},
homeTeamScore: 0,
visitingTeamScore: 5,
finishedTimeStatus: "ORDINARY_TIME",
league: {
id: 55193,
name: "Premier League"
}
}
]
}
