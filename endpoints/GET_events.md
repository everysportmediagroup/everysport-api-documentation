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
    "credit": {
        "link": "http://www.everysport.com", 
        "logoUrl": "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png", 
        "message": "Provided by Everysport.com"
    }, 
    "events": [
        {
            "homeTeam": {
                "id": 28065, 
                "link": "http://www.everysport.com/sport/ishockey/team/boston-bruins/28065", 
                "name": "Boston Bruins", 
                "shortName": "Boston"
            }, 
            "id": 2136643, 
            "league": {
                "id": 58878, 
                "name": "NHL", 
                "sport": {
                    "id": 2, 
                    "name": "Ishockey"
                }
            }, 
            "round": 35, 
            "startDate": "2013-04-03T01:00+0200", 
            "status": "UPCOMING", 
            "visitingTeam": {
                "id": 28050, 
                "link": "http://www.everysport.com/sport/ishockey/team/ottawa-senators/28050", 
                "name": "Ottawa Senators", 
                "shortName": "Ottawa"
            }
        }, 
        {
            "homeTeam": {
                "id": 28052, 
                "link": "http://www.everysport.com/sport/ishockey/team/new-york-islanders/28052", 
                "name": "New York Islanders", 
                "shortName": "NY Islanders"
            }, 
            "id": 2136644, 
            "league": {
                "id": 58878, 
                "name": "NHL", 
                "sport": {
                    "id": 2, 
                    "name": "Ishockey"
                }
            }, 
            "round": 35, 
            "startDate": "2013-04-03T01:00+0200", 
            "status": "UPCOMING", 
            "visitingTeam": {
                "id": 109005, 
                "link": "http://www.everysport.com/sport/ishockey/team/winnipeg-jets/109005", 
                "name": "Winnipeg Jets", 
                "shortName": "Winnipeg"
            }
        }, 
        {
            "homeTeam": {
                "id": 28056, 
                "link": "http://www.everysport.com/sport/ishockey/team/carolina-hurricanes/28056", 
                "name": "Carolina Hurricanes", 
                "shortName": "Carolina"
            }, 
            "id": 2136645, 
            "league": {
                "id": 58878, 
                "name": "NHL", 
                "sport": {
                    "id": 2, 
                    "name": "Ishockey"
                }
            }, 
            "round": 35, 
            "startDate": "2013-04-03T01:00+0200", 
            "status": "UPCOMING", 
            "visitingTeam": {
                "id": 28073, 
                "link": "http://www.everysport.com/sport/ishockey/team/washington-capitals/28073", 
                "name": "Washington Capitals", 
                "shortName": "Washington"
            }
        }
    ], 
    "metadata": {
        "count": 3, 
        "limit": 3, 
        "offset": 0, 
        "totalCount": 189
    }
}
```
