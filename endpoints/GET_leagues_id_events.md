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
* limit - limits the number of events, positive integer
* offset - indicates where to start in the list. Defaults to 0, positive integer
* sort - the property and order by which the events is sorted. Can be 'startDate:asc', 'startDate:desc', 'round:asc' or 'round:desc'. Default is 'startDate:asc'.
* team - a comma-separated list of one or many team IDs, for which to retrieve events.  
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esEvents'.
* municipality - filters out events in a given municipality. Use 'municipality', 'homeTeam.municipality' or 'visitingTeam.municipality'. Use a comma-separated list to get events from two or more municipalities.


## Example Request
```
GET http://api.everysport.com/v1/leagues/63925/events?limit=2&status=upcoming
```

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
        "totalCount": 144,
        "offset": 0
    },
    "events": [
        {
            "id": 2324311,
            "links": [
                {
                    "rel": "self",
                    "href": "http://api.everysport.com/v1/events/2324311"
                }
            ],
            "startDate": "2014-07-05T16:00+0200",
            "round": 13,
            "status": "UPCOMING",
            "homeTeam": {
                "id": 9374,
                "name": "Kalmar FF",
                "shortName": "Kalmar FF",
                "link": "http://www.everysport.com/sport/fotboll/team/kalmar-ff/9374",
                "municipality": {
                    "id": 880,
                    "name": "Kalmar"
                }
            },
            "visitingTeam": {
                "id": 9389,
                "name": "Mjällby AIF",
                "shortName": "Mjällby",
                "link": "http://www.everysport.com/sport/fotboll/team/mjaellby-aif/9389",
                "municipality": {
                    "id": 1083,
                    "name": "Sölvesborg"
                }
            },
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
                    "id": 63057,
                    "name": "Guldfågeln Arena"
                }
            }
        },
        {
            "id": 2324312,
            "links": [
                {
                    "rel": "self",
                    "href": "http://api.everysport.com/v1/events/2324312"
                }
            ],
            "startDate": "2014-07-05T16:00+0200",
            "round": 13,
            "status": "UPCOMING",
            "homeTeam": {
                "id": 9381,
                "name": "Falkenbergs FF",
                "shortName": "Falkenberg",
                "link": "http://www.everysport.com/sport/fotboll/team/falkenbergs-ff/9381",
                "municipality": {
                    "id": 1382,
                    "name": "Falkenberg"
                }
            },
            "visitingTeam": {
                "id": 9371,
                "name": "Halmstads BK",
                "shortName": "Halmstad",
                "link": "http://www.everysport.com/sport/fotboll/team/halmstads-bk/9371",
                "municipality": {
                    "id": 1380,
                    "name": "Halmstad"
                }
            },
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
                    "id": 60659,
                    "name": "Falkenbergs IP"
                }
            }
        }
    ]
}
```
