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

## Return format
An object with the following keys and values:
* credits - a Credit object
* events - a list of Event objects

```javascript
{
  "credits":{...},
  "events":[{
    "id": 1, //Unique event id
    "startDate":"2001-02-03T04:05+01:00", //Using ISO 8601 http://sv.wikipedia.org/wiki/ISO_8601
    "status":"finished", //Possible values are: upcoming, postponed, ongoing, finished (future support: cancelled)
    "visitingTeamScore":5, //Reflects the score dependent on the event status. E.g. an upcoming event has score set to null
    "homeTeamScore":4,
    "visitingTeam":{...},
    "homeTeam":{...},
    "round": 14 //Indicates league round this event belongs to
  },
  {...}
  ]
}
```
