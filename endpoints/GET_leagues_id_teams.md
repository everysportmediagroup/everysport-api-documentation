# Teams

    GET leagues/:id/teams

## Description
Returns a list of Team objects for the league.

## Resource URL

		http://api.everysport.com/v1/leagues/:id/teams


## Parameters
* id (required) - the League ID
* apikey (required) - your APIKEY
* facts - boolean, filter teams with facts (goals).
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esTeams'.


## Example Request
```
GET http://api.everysport.com/v1/leagues/74542/teams?facts=true
```

```javascript
{
  "credit": {
    "message": "Provided by Everysport.com",
    "link": "http://www.everysport.com",
    "logoUrl": "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png"
  },
  metadata: {
    count: 2
  },
  teams: [
    {
      id: 58582,
      name: "Hovshaga AIF",
      shortName: "Hovshaga",
      abbreviation: "Hovshaga",
      facts: true
    },
    {
      id: 58580,
      name: "IBK Vöikers",
      shortName: "Vöikers",
      abbreviation: "Vöikers",
      facts: true
    }
  ]
}
```
