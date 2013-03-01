# Search

    GET search

## Description
Searches Sports, Teams and Leagues based on their respective names. For Leagues, the name of the league as well as the names of all groups within the league, are searched. 

A match is found if the text in the 'q' parameter is anywhere inside the name. For example, q=hockey will match the sport "ice hockey", the league "sweden hockey games" and the team "Modo Hockey".     

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
	'leagues' : [ 
			{	name: '', id: , group: {name: '', id: }},
		 … 
	]
}  