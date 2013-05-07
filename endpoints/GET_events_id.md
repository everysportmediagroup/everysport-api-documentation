# Search

    GET events/:id

## Description
Get detailed information about an event   

## Parameters
* id (required) - the Event ID
* apikey (required) - your APIKEY

## Return format

```javascript	

{
    "credit": {
        "link": "http://www.everysport.com", 
        "logoUrl": "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png", 
        "message": "Provided by Everysport.com"
    }, 
    "event": {
	"homeTeam": {
        	"id": 28065, 
                "link": "http://www.everysport.com/sport/ishockey/team/boston-bruins/28065", 
                "name": "Boston Bruins", 
                "shortName": "Boston"
         }, 
         "id": 2136643, 
         "league": {
         	"id": 58878, 
                "name": "NHL", 
                "sport": {
                    "id": 2, 
                    "name": "Ishockey"
                }
         }, 
         "round": 35, 
         "startDate": "2013-04-03T01:00+0200", 
         "status": "FINISHED", 
         "visitingTeam": {
              "id": 28050, 
               "link": "http://www.everysport.com/sport/ishockey/team/ottawa-senators/28050", 
               "name": "Ottawa Senators", 
               "shortName": "Ottawa"
          },
          "facts" : {
 	    	"spectators": 7659,    	
    		"arena" : {
    			"id" : 31,
	    		"name": "Malmö Stadion",
    		},
	    	"referees" : ["Chuck Norris", "Jackie Chan"],
	  },
	  "gameEventLevel": "DETAILED",
	  "gameEvents" : [		
    		{
    			"level" :"DETAILED",
			"minute":2,
			"second": 0,
			"count": 1,
			"penaltyShot": 1,
	    		"type" : "GOAL"    		
			"team" : {
        			"id": 28065, 
		                "link": "http://www.everysport.com/sport/ishockey/team/boston-bruins/28065", 
                		"name": "Boston Bruins", 
		                "shortName": "Boston"
		        },
	    		"player" : {
	    			"name" : "Peter Forsberg",

	    		},
			"assistingPlayers": [{
	    			"name" : "Markus Näslund",

	    		}, {
	    			"name" : "Peter Forsberg",

	    		}],			
	    		"homeTeamScore":2,
	    		"visitingTeamScore":3
    		},
    		{
    			"level" :"DETAILED",
    			"minute":2,
			"second": 0,
	    		"type" : "PENALTY_WARNING",
	    		"team" : {
        			"id": 28065, 
		                "link": "http://www.everysport.com/sport/ishockey/team/boston-bruins/28065", 
                		"name": "Boston Bruins", 
		                "shortName": "Boston"
		        },
	    		"player" : {
	    			"name" : "Peter Forsberg",

	    		}
	    			    	
    		},
    		{
			"team": {
				"id": 1208,
				"name": "Hammarby IF",
				"shortName": "Hammarby",			
			},
			"count": 1,
			"type": "PENALTY",
			"penaltyType": "TEN_MIN",
			"level": "AGGREGATED"
		}
    	],
    	"periodResults" : [
    		{	
			"type" : "PERIOD_RESULT",
			"period": 1,
			"homeTeamPeriodScore": 1,
	    		"visitingTeamPeriodScore": 3
		},
		{
			"type" : "ORDINARY_TIME_RESULT",
			"homeTeamScore": 1,
	    		"visitingTeamScore": 3
		}],
	"subGames" : [
		{
			"gameNumber": 1,
			"homeTeam": {
				"id": 1,
				"name": "Halmstad"
			},
			"homeTeamPlayer": {
				"name": "..."
			},
			"visitingTeam": {
				"id": 1,
				"name": "Alingsås"
			},
			"visitingTeamPlayer": {
				"name": "..."
			},
			"scores" : [ 
				{
					"homeTeamScore": 11,
					"visitingTeamScore": 8,
				}, { ...} 
			]
		}
	]	
    }
}
```
	
