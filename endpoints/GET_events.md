# Events

    GET events

## Description
Returns a list of Event objects.  

## Parameters
* apikey (required) - your APIKEY
* league - a comma-separated list of league IDs, for which to retrieve events.
* status - a comma-seperated list of one or many status, for which to retrieve events. Can be any status value as defined by the Event object.
* fromDate - filters out events after a specific date, Date in short format
* toDate - filters out events before a specific date, Date in short format
* round - a comma-seperated list of one or many rounds, for which to retrieve events.
* limit - limits the number of events, positive integer
* offset - indicates where to start in the list. Defaults to 0, positive integer
* sort - the property and order by which the events is sorted. Can be 'startDate:asc', 'startDate:desc', 'round:asc' or 'round:desc'. Default is 'startDate:asc'.
* team - a comma-separated list of one or many team IDs, for which to retrieve events.  
* sport - a comma-separated list of one or many sport IDs, for which to retrieve events.  
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esEvents'
* fields - include detailed data about events. Can be 'all'.
* municipality - filters out events in a given municipality. Use 'municipality', 'homeTeam.municipality' or 'visitingTeam.municipality'. Use a comma-separated list to get events from two or more municipalities.

## Return format

```javascript	
{
    "credit": {
        "message": "Provided by Everysport.com",
        "link": "http://www.everysport.com",
        "logoUrl": "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png"
    },
    "metadata": {
        "limit": 2,
        "count": 2,
        "totalCount": 240,
        "offset": 0
    },
    "events": [
        {
            "id": 2324212,
            "links": [
                {
                    "rel": "self",
                    "href": "http://api.everysport.com/v1/events/2324212"
                }
            ],
            "startDate": "2014-03-30T15:00+0200",
            "round": 1,
            "status": "FINISHED",
            "homeTeam": {
                "id": 19721,
                "name": "IF Brommapojkarna",
                "shortName": "Brommapojk",
                "link": "http://www.everysport.com/sport/fotboll/team/if-brommapojkarna/19721",
                "municipality": {
                    "id": 180,
                    "name": "Stockholm"
                }
            },
            "visitingTeam": {
                "id": 9374,
                "name": "Kalmar FF",
                "shortName": "Kalmar FF",
                "link": "http://www.everysport.com/sport/fotboll/team/kalmar-ff/9374",
                "municipality": {
                    "id": 880,
                    "name": "Kalmar"
                }
            },
            "homeTeamScore": 1,
            "visitingTeamScore": 2,
            "finishedTimeStatus": "ORDINARY_TIME",
            "league": {
                "id": 63925,
                "links": [
                    {
                        "rel": "self",
                        "href": "http://api.everysport.com/v1/leagues/63925"
                    }
                ],
                "name": "Allsvenskan",
                "level": "Allsvenskan",
                "sport": {
                    "id": 10,
                    "links": [
                        {
                            "rel": "self",
                            "href": "http://api.everysport.com/v1/sports/10"
                        }
                    ],
                    "name": "Fotboll"
                },
                "teamClass": "MEN",
                "startDate": "2014-03-30T00:00+0100",
                "endDate": "2014-11-02T00:00+0100"
            },
            "facts": {
                "arena": {
                    "id": 110295,
                    "name": "Grimsta IP 1"
                },
                "spectators": 2028
            }
        },
        {
            "id": 2324213,
            "links": [
                {
                    "rel": "self",
                    "href": "http://api.everysport.com/v1/events/2324213"
                }
            ],
            "startDate": "2014-03-30T15:00+0200",
            "round": 1,
            "status": "FINISHED",
            "homeTeam": {
                "id": 9389,
                "name": "Mjällby AIF",
                "shortName": "Mjällby",
                "link": "http://www.everysport.com/sport/fotboll/team/mjaellby-aif/9389",
                "municipality": {
                    "id": 1083,
                    "name": "Sölvesborg"
                }
            },
            "visitingTeam": {
                "id": 9400,
                "name": "Gefle IF",
                "shortName": "Gefle",
                "link": "http://www.everysport.com/sport/fotboll/team/gefle-if/9400",
                "municipality": {
                    "id": 2180,
                    "name": "Gävle"
                }
            },
            "homeTeamScore": 2,
            "visitingTeamScore": 2,
            "finishedTimeStatus": "ORDINARY_TIME",
            "league": {
                "id": 63925,
                "links": [
                    {
                        "rel": "self",
                        "href": "http://api.everysport.com/v1/leagues/63925"
                    }
                ],
                "name": "Allsvenskan",
                "level": "Allsvenskan",
                "sport": {
                    "id": 10,
                    "links": [
                        {
                            "rel": "self",
                            "href": "http://api.everysport.com/v1/sports/10"
                        }
                    ],
                    "name": "Fotboll"
                },
                "teamClass": "MEN",
                "startDate": "2014-03-30T00:00+0100",
                "endDate": "2014-11-02T00:00+0100"
            },
            "facts": {
                "arena": {
                    "id": 61382,
                    "name": "Strandvallen"
                },
                "spectators": 3532
            }
        }
    ]
}
```
