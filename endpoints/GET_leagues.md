# Search

    GET leagues

## Description
Returns a list of all League Objects available for the given APIKEY. 

Use the 'sport' parameter to limit the result to leagues for specific sports.     

## Parameters
* apikey (required) - your APIKEY
* sport (optional) - comma separated list of sports to retrieve leagues for, for example 'bandy,speedway'
* limit (optional) - Limits the number of items trying to retrieve, positive integer
* offset - Indicates where to start in the list. Defaults to 0, positive integer

## Return format
```javascript	
{ credit: {},
	leagues: [
	{'name': …,
	 'id': …,
	 'sport': …
	}

	]
}  