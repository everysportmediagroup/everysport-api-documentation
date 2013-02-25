# Search

    GET search

## Description
Searches sports, leagues and teams on everysport.com.

## Parameters
* apikey (required) - your APIKEY
* q (required) - the search query, string
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 

## Return format

```javascript	
{ 
	'credits': {...} ,
	'sports': [{name: '', id:  }, … ],
	'teams' : [{ { name: '', id:   }, … ],
	'leagues' : [ { name: '', id: }, … ]
}  