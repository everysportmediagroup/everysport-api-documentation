# Event

    GET events/:id

## Description
Returns basic information about a specific event, such as location, teams and audience. 

Live reports and chat are available as sub-resources. 

The Event ID is available, for example, inside [/leagues/:id/events](GET_leagues_id_events.md). 

## Parameters
* apikey (required) - your APIKEY
* id (required) - the event ID, int
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 

## Return format

```javascript	
{ 
	'credits': {...}, //A Credits object
	'event': {}, //An Event object
	'everysport': {
				url: '', //URL to event page on everysport.com
				audience: ,//number of people connected to the event
			},
	'location' : {lat:,log:}
					
}
