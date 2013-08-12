# Leagues

    GET leagues

## Description
Returns a list of all League Objects available for the given APIKEY. 

Use the 'sport' parameter to limit the result to leagues for specific sports.     

## Parameters
* apikey (required) - your APIKEY
* sport (optional) - comma separated list of sport ID to retrieve leagues for, for example 10 is football and 2 is ice hockey. 
* teamClass (optional) - comma separated list of team classes to retrieve leagues for, for example 'men,women'
* country (optional) - country to retrive leagues for, support only 'se' (Sweden) as country.
* limit (optional) - Limits the number of items trying to retrieve, positive integer
* offset (optiona) - Indicates where to start in the list. Defaults to 0, positive integer

## Example Request
```
GET /leagues
```

```javascript	
{
    credit: {
        message: "Provided by Everysport.com",
        link: "http://www.everysport.com",
        logoUrl: "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png"
    },
    metadata: {
        limit: 50,
        count: 7,
        totalCount: 7,
        offset: 0
    },
    leagues: [
        {
            id: 3,
            name: "...",
            teamClass: "men",
            sport: {
            	id: 2,
            	name: "Fotboll"
            }
        },
        ....
    ]
}
