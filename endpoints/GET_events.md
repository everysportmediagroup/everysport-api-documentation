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
{ "credit" : { "link" : "http://www.everysport.com",
      "logoUrl" : "http://c.static.es-cdn.net/files/everysport2/images/  icons/event/small/everysport.png",
      "message" : "Provided by Everysport.com"
    },
  "events" : [ { "finishedTimeStatus" : "ORDINARY_TIME",
        "homeTeam" : { "id" : 27681,
            "link" : "http://www.everysport.com/sport/fotboll/team/arsenal/27681",
            "name" : "Arsenal",
            "shortName" : "Arsenal"
          },
        "homeTeamScore" : 0,
        "id" : 2044519,
        "league" : { "id" : 55193,
            "name" : "Premier League"
          },
        "round" : 1,
        "startDate" : "2012-08-18T15:00+0200",
        "status" : "FINISHED",
        "visitingTeam" : { "id" : 27669,
            "link" : "http://www.everysport.com/sport/fotboll/team/sunderland/27669",
            "name" : "Sunderland",
            "shortName" : "Sunderland"
          },
        "visitingTeamScore" : 0
      },
      { "finishedTimeStatus" : "ORDINARY_TIME",
        "homeTeam" : { "id" : 27675,
            "link" : "http://www.everysport.com/sport/fotboll/team/fulham/27675",
            "name" : "Fulham",
            "shortName" : "Fulham"
          },
        "homeTeamScore" : 5,
        "id" : 2044520,
        "league" : { "id" : 55193,
            "name" : "Premier League"
          },
        "round" : 1,
        "startDate" : "2012-08-18T15:00+0200",
        "status" : "FINISHED",
        "visitingTeam" : { "id" : 27703,
            "link" : "http://www.everysport.com/sport/fotboll/team/norwich/27703",
            "name" : "Norwich",
            "shortName" : "Norwich"
          },
        "visitingTeamScore" : 0
      },
      { "finishedTimeStatus" : "ORDINARY_TIME",
        "homeTeam" : { "id" : 27694,
            "link" : "http://www.everysport.com/sport/fotboll/team/queens-pr/27694",
            "name" : "Queens PR",
            "shortName" : "QPR"
          },
        "homeTeamScore" : 0,
        "id" : 2044521,
        "league" : { "id" : 55193,
            "name" : "Premier League"
          },
        "round" : 1,
        "startDate" : "2012-08-18T15:00+0200",
        "status" : "FINISHED",
        "visitingTeam" : { "id" : 27711,
            "link" : "http://www.everysport.com/sport/fotboll/team/swansea/27711",
            "name" : "Swansea",
            "shortName" : "Swansea"
          },
        "visitingTeamScore" : 5
      }
    ],
  "metadata" : { "count" : 3,
      "limit" : 3,
      "offset" : 0,
      "totalCount" : 914
    }
}
```
