# Standings

    GET leagues/:id/standings

## Description
Returns a list of the current standings (i.e. the tables) for the league. 

A league may contain one or many groups. For example, the NHL league has several groups, such as the conferences (Eastern and Western) and divisions (Atlantic, Pacific, etc.). One team may belong to more than one group. Most leagues, however, has only one group. 

The league standings, commonly visualized as a table, is essentially a list of the teams and their respective stats, sorted by one of the stats attributes, normally the total points. 

## Parameters
* id (required) - The League ID
* apikey (required) - your APIKEY
* type - one of 'total' (default), 'home' and 'away' 
* size - specifies the amount of statistics data for the teams. Default is 'large' which retrieves all available data. Use  'medium' and 'small' to get less data. 
* sortKey - the key by which the standings is sorted. Can be any of the attribute names from the Team Stats objects (eg. 'stats.pts') or 'team.name' to sort by the name of the team. By default, sorting is by 'stats.pts'.   
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 

## Return format
An object with the following keys and values:
* credits - a Credits object
* groups - a list of one or many Groups objects.   

### Group object
A Group object has the following data: 
* labels - an ordered array of objects containing type and name
* standings - a list of Standings objects

### Standings object
A Standings object has the following data: 
* team - a Team Object in short format
* stats - an array of Team Stats Object

## Examples

### NHL
```javascript	
{ 
	'credits': {...} ,
	'groups': [
  	  { 
  	    'labels:' [ {'type' : 'conference', 'name' : 'Western Conference' }, {'type' : 'division', 'name' : 'Central Division' }],
  	    'standings' : [
  	    	{
  	    	  'team' : {
  	    	    'name':'Super Great Team Name',
  	    	    ...
  	    	  },
  	    	  'stats' : [
  	    	    {'name':'gp', 'value':12},
  	    	    {'name':'w', 'value':5},
  	    	    {'name':'l', 'value':4},
  	    	    ...
  	    	  ]	
  	    	},
  	    	{
  	    	  'team' : {
  	    	    'name':'Super Great Team Name',
  	    	    ...
  	    	  },
  	    	  'stats' : [
  	    	    {'name':'gp', 'value':12},
  	    	    {'name':'w', 'value':5},
  	    	    {'name':'l', 'value':4}
  	    	    ...
  	    	  ]	
  	    	}]
  	  },
  	  ...
  	]
}
```
            

### Bowling - Division 1
```javascript
{ 
  'credits': {..} ,
  'groups': [
  	{ 
  	'labels:' [ {'type' : group'name' : 'A' }],
  	'standings' : [{
		'team' : { ... }
        	'stats' : [
        		  {...}, 
        		  {...},
        		  ...
        		]
        	},
        	{...}
        	]
        }]
}
```

### Elitserien
	
```javascript
{ 
  'credits': {..} ,
  'groups': [
  	{ 
  	'labels:' [],
  	'standings' : [{
		'team' : {...}
        	'stats' : [
        		{...},
        		{...}
        		]
        	},
        	{...}
        	]
        }]
}
```


	
        	
