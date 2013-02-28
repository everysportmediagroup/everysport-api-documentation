# Sports

    GET sports

## Description
Returns a list of all Sport Objects available for the given APIKEY.

List is sorted by name.

## Parameters
* apikey (required) - your APIKEY
* limit (optional) - Limits the number of items trying to retrieve, positive integer
* offset (optional) - Indicates where to start in the list. Defaults to 0, positive integer 

## Example Request
```
GET /sports
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
    sports: [
        {
            id: 3,
            name: "Bandy"
        },
        {
            id: 5,
            name: "Basket"
        },
        {
            id: 10,
            name: "Fotboll"
        },
        {
            id: 7,
            name: "Handboll"
        },
        {
            id: 4,
            name: "Innebandy"
        },
        {
            id: 2,
            name: "Ishockey"
        },
        {
            id: 15,
            name: "Speedway"
        }
    ]
}
