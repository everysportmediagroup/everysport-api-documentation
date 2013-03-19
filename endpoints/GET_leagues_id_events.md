# Events

    GET leagues/:id/events

## Description
Returns a list of Event objects for the league.

## Resource URL

		http://api.everysport.com/v1/leagues/:id/events


## Parameters
* id (required) - the League ID
* apikey (required) - your APIKEY
* status - a comma-seperated list of one or many status, for which to retrieve events. Can be any status value as defined by the Event object.
* fromDate - filters out events after a specific date, Date in short format
* toDate - filters out events before a specific date, Date in short format
* round - a comma-seperated list of one or many rounds, for which to retrieve events.
* limit - Limits the number of events, positive integer
* offset - Indicates where to start in the list. Defaults to 0, positive integer
* sort - the property and order by which the events is sorted. Can be 'startDate:asc', 'startDate:desc', 'round:asc' or 'round:desc'. Default is 'startDate:asc'.
* team - a comma-separated list of one or many team IDs, for which to retrieve events.  
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esEvents'


## Example Request
```
GET http://api.everysport.com/v1/leagues/58878/events?limit=10&status=upcoming
```

```javascript
{
    "credit": {
        "link": "http://www.everysport.com", 
        "logoUrl": "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png", 
        "message": "Provided by Everysport.com"
    }, 
    "events": [
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28069, 
                "link": "http://www.everysport.com/sport/ishockey/team/philadelphia/28069", 
                "shortName": "Philadelphia"
            }, 
            "homeTeamScore": 1, 
            "id": 2135253, 
            "round": 1, 
            "startDate": "2013-01-19T01:00+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28062, 
                "link": "http://www.everysport.com/sport/ishockey/team/pittsburgh/28062", 
                "shortName": "Pittsburgh"
            }, 
            "visitingTeamScore": 3
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28066, 
                "link": "http://www.everysport.com/sport/ishockey/team/montreal/28066", 
                "shortName": "Montreal"
            }, 
            "homeTeamScore": 1, 
            "id": 2135257, 
            "round": 1, 
            "startDate": "2013-01-19T01:00+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28049, 
                "link": "http://www.everysport.com/sport/ishockey/team/toronto/28049", 
                "shortName": "Toronto"
            }, 
            "visitingTeamScore": 2
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28052, 
                "link": "http://www.everysport.com/sport/ishockey/team/ny-islanders/28052", 
                "shortName": "NY Islanders"
            }, 
            "homeTeamScore": 1, 
            "id": 2135258, 
            "round": 1, 
            "startDate": "2013-01-19T01:00+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28061, 
                "link": "http://www.everysport.com/sport/ishockey/team/new-jersey/28061", 
                "shortName": "New Jersey"
            }, 
            "visitingTeamScore": 2
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28065, 
                "link": "http://www.everysport.com/sport/ishockey/team/boston/28065", 
                "shortName": "Boston"
            }, 
            "homeTeamScore": 3, 
            "id": 2135256, 
            "round": 1, 
            "startDate": "2013-01-19T01:30+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28070, 
                "link": "http://www.everysport.com/sport/ishockey/team/ny-rangers/28070", 
                "shortName": "NY Rangers"
            }, 
            "visitingTeamScore": 1
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28055, 
                "link": "http://www.everysport.com/sport/ishockey/team/tampa-bay/28055", 
                "shortName": "Tampa Bay"
            }, 
            "homeTeamScore": 6, 
            "id": 2135259, 
            "round": 1, 
            "startDate": "2013-01-19T01:30+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28073, 
                "link": "http://www.everysport.com/sport/ishockey/team/washington/28073", 
                "shortName": "Washington"
            }, 
            "visitingTeamScore": 3
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28047, 
                "link": "http://www.everysport.com/sport/ishockey/team/florida/28047", 
                "shortName": "Florida"
            }, 
            "homeTeamScore": 5, 
            "id": 2135260, 
            "round": 1, 
            "startDate": "2013-01-19T01:30+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28056, 
                "link": "http://www.everysport.com/sport/ishockey/team/carolina/28056", 
                "shortName": "Carolina"
            }, 
            "visitingTeamScore": 1
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28057, 
                "link": "http://www.everysport.com/sport/ishockey/team/minnesota/28057", 
                "shortName": "Minnesota"
            }, 
            "homeTeamScore": 4, 
            "id": 2135264, 
            "round": 1, 
            "startDate": "2013-01-19T02:00+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28054, 
                "link": "http://www.everysport.com/sport/ishockey/team/colorado/28054", 
                "shortName": "Colorado"
            }, 
            "visitingTeamScore": 2
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28059, 
                "link": "http://www.everysport.com/sport/ishockey/team/dallas/28059", 
                "shortName": "Dallas"
            }, 
            "homeTeamScore": 4, 
            "id": 2135263, 
            "round": 1, 
            "startDate": "2013-01-19T02:30+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28064, 
                "link": "http://www.everysport.com/sport/ishockey/team/phoenix/28064", 
                "shortName": "Phoenix"
            }, 
            "visitingTeamScore": 3
        }, 
        {
            "finishedTimeStatus": "PENALTY_SHOOTOUT", 
            "homeTeam": {
                "id": 28067, 
                "link": "http://www.everysport.com/sport/ishockey/team/nashville/28067", 
                "shortName": "Nashville"
            }, 
            "homeTeamScore": 2, 
            "id": 2135262, 
            "round": 1, 
            "startDate": "2013-01-19T03:00+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28074, 
                "link": "http://www.everysport.com/sport/ishockey/team/columbus/28074", 
                "shortName": "Columbus"
            }, 
            "visitingTeamScore": 3
        }, 
        {
            "finishedTimeStatus": "ORDINARY_TIME", 
            "homeTeam": {
                "id": 28058, 
                "link": "http://www.everysport.com/sport/ishockey/team/calgary/28058", 
                "shortName": "Calgary"
            }, 
            "homeTeamScore": 1, 
            "id": 2135267, 
            "round": 1, 
            "startDate": "2013-01-19T03:30+01", 
            "status": "FINISHED", 
            "visitingTeam": {
                "id": 28068, 
                "link": "http://www.everysport.com/sport/ishockey/team/san-jose/28068", 
                "shortName": "San Jose"
            }, 
            "visitingTeamScore": 4
        }
    ], 
    "metadata": {
        "count": 10, 
        "limit": 10, 
        "offset": 0, 
        "totalCount": 713
    }
}
```
