# Design Principles
At Menmo we do our best to craft a world-class API developers will love. To do that, we follow these design principles:

## Versioning
We put version at the top of the URI. 

	/v1/.. 
	/v2/..

## Formats
Currently only JSON is supported as the return format. 

We may add XML or others in the future, using ".xml" and ".json" extensions. 

## JSON-P
Almost every call supports the 'callback' parameter to enable so called JSON-P. 


## Pagination
We use 'offset' and 'limit' parameters to return a slice of a longer list. 

	/leagues/54258/events?offset=10&limit=10

## Search
Where search is supported, we use the "q" parameter. 

	/players?q=zlatan

Returns all players who's name contain "Zlatan".

## Sorting
Where sorting is supported, we use the "sort" parameter with the name of the key to sort on.

Descending: 

	leagues/54258/events?sort=startDate:desc

Ascending:

	leagues/54258/events?sort=startDate:sac

## Errors
We use a few HTTP response codes to indicate when something went wrong: 

- 200 - OK
- 400 - Bad Request, client did something wrong
- 404 - Not Found, no content
- 405 - Method not allowed
- 500 - Internal Server Error, server did something wrong








 



