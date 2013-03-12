# Standings

	GET leagues/:id/standings

## Description
Returns a list of the current standings (i.e. the tables) for the league. 

A league may contain one or many groups. For example, the NHL league has several groups, such as the conferences (Eastern and Western) and divisions (Atlantic, Pacific, etc.). One team may belong to more than one group. Most leagues, however, has only one group. 

The league standings, commonly visualized as a table, is essentially a list of the teams and their respective stats, sorted by one of the stats attributes, normally the total points. 


## Resource URL

	http://api.everysport.com/v1/leagues/id:/standings


## Parameters
* id (required) - The League ID
* apikey (required) - your APIKEY
* type - one of 'total' (default), 'home' and 'away' 
* size - specifies the amount of statistics data for the teams. Default is 'large' which retrieves all available data. Use  'medium' and 'small' to get less data. 
* sortKey - the key by which the standings is sorted. Can be any of the attribute names from the Team Stats objects (eg. 'stats.pts') or 'team.name' to sort by the name of the team. By default, sorting is by 'stats.pts'.   
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 


## Example Request

	GET http://api.everysport.com/v1/leagues/58878/standings


```javascript	
{
    "credit": {
        "link": "http://www.everysport.com", 
        "logoUrl": "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png", 
        "message": "Provided by Everysport.com"
    }, 
    "groups": [
        {
            "labels": [
                {
                    "name": "Western Conference", 
                    "type": "conference"
                }, 
                {
                    "name": "Central Division", 
                    "type": "division"
                }
            ], 
            "standings": [
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 17
                        }, 
                        {
                            "name": "l", 
                            "value": 0
                        }, 
                        {
                            "name": "gf", 
                            "value": 64
                        }, 
                        {
                            "name": "ga", 
                            "value": 37
                        }, 
                        {
                            "name": "gd", 
                            "value": 27
                        }, 
                        {
                            "name": "pts", 
                            "value": 37
                        }
                    ], 
                    "team": {
                        "id": 28075, 
                        "link": "http://www.everysport.com/sport/ishockey/team/chicago-blackhawks/28075", 
                        "name": "Chicago Blackhawks", 
                        "shortName": "Chicago"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 21
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 8
                        }, 
                        {
                            "name": "gf", 
                            "value": 60
                        }, 
                        {
                            "name": "ga", 
                            "value": 57
                        }, 
                        {
                            "name": "gd", 
                            "value": 3
                        }, 
                        {
                            "name": "pts", 
                            "value": 23
                        }
                    ], 
                    "team": {
                        "id": 28071, 
                        "link": "http://www.everysport.com/sport/ishockey/team/detroit-red-wings/28071", 
                        "name": "Detroit Red Wings", 
                        "shortName": "Detroit"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 21
                        }, 
                        {
                            "name": "w", 
                            "value": 9
                        }, 
                        {
                            "name": "l", 
                            "value": 7
                        }, 
                        {
                            "name": "gf", 
                            "value": 45
                        }, 
                        {
                            "name": "ga", 
                            "value": 52
                        }, 
                        {
                            "name": "gd", 
                            "value": -7
                        }, 
                        {
                            "name": "pts", 
                            "value": 23
                        }
                    ], 
                    "team": {
                        "id": 28067, 
                        "link": "http://www.everysport.com/sport/ishockey/team/nashville-predators/28067", 
                        "name": "Nashville Predators", 
                        "shortName": "Nashville"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 7
                        }, 
                        {
                            "name": "gf", 
                            "value": 55
                        }, 
                        {
                            "name": "ga", 
                            "value": 55
                        }, 
                        {
                            "name": "gd", 
                            "value": 0
                        }, 
                        {
                            "name": "pts", 
                            "value": 22
                        }
                    ], 
                    "team": {
                        "id": 28072, 
                        "link": "http://www.everysport.com/sport/ishockey/team/st-louis-blues/28072", 
                        "name": "St Louis Blues", 
                        "shortName": "St Louis"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 5
                        }, 
                        {
                            "name": "l", 
                            "value": 12
                        }, 
                        {
                            "name": "gf", 
                            "value": 44
                        }, 
                        {
                            "name": "ga", 
                            "value": 61
                        }, 
                        {
                            "name": "gd", 
                            "value": -17
                        }, 
                        {
                            "name": "pts", 
                            "value": 13
                        }
                    ], 
                    "team": {
                        "id": 28074, 
                        "link": "http://www.everysport.com/sport/ishockey/team/columbus-blue-jackets/28074", 
                        "name": "Columbus Blue Jackets", 
                        "shortName": "Columbus"
                    }
                }
            ]
        }, 
        {
            "labels": [
                {
                    "name": "Western Conference", 
                    "type": "conference"
                }, 
                {
                    "name": "Northwest Division", 
                    "type": "division"
                }
            ], 
            "standings": [
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 5
                        }, 
                        {
                            "name": "gf", 
                            "value": 54
                        }, 
                        {
                            "name": "ga", 
                            "value": 52
                        }, 
                        {
                            "name": "gd", 
                            "value": 2
                        }, 
                        {
                            "name": "pts", 
                            "value": 24
                        }
                    ], 
                    "team": {
                        "id": 28063, 
                        "link": "http://www.everysport.com/sport/ishockey/team/vancouver-canucks/28063", 
                        "name": "Vancouver Canucks", 
                        "shortName": "Vancouver"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 7
                        }, 
                        {
                            "name": "gf", 
                            "value": 43
                        }, 
                        {
                            "name": "ga", 
                            "value": 46
                        }, 
                        {
                            "name": "gd", 
                            "value": -3
                        }, 
                        {
                            "name": "pts", 
                            "value": 22
                        }
                    ], 
                    "team": {
                        "id": 28057, 
                        "link": "http://www.everysport.com/sport/ishockey/team/minnesota-wild/28057", 
                        "name": "Minnesota Wild", 
                        "shortName": "Minnesota"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 8
                        }, 
                        {
                            "name": "l", 
                            "value": 7
                        }, 
                        {
                            "name": "gf", 
                            "value": 47
                        }, 
                        {
                            "name": "ga", 
                            "value": 50
                        }, 
                        {
                            "name": "gd", 
                            "value": -3
                        }, 
                        {
                            "name": "pts", 
                            "value": 20
                        }
                    ], 
                    "team": {
                        "id": 28053, 
                        "link": "http://www.everysport.com/sport/ishockey/team/edmonton-oilers/28053", 
                        "name": "Edmonton Oilers", 
                        "shortName": "Edmonton"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 8
                        }, 
                        {
                            "name": "l", 
                            "value": 8
                        }, 
                        {
                            "name": "gf", 
                            "value": 49
                        }, 
                        {
                            "name": "ga", 
                            "value": 58
                        }, 
                        {
                            "name": "gd", 
                            "value": -9
                        }, 
                        {
                            "name": "pts", 
                            "value": 19
                        }
                    ], 
                    "team": {
                        "id": 28054, 
                        "link": "http://www.everysport.com/sport/ishockey/team/colorado-avalanche/28054", 
                        "name": "Colorado Avalanche", 
                        "shortName": "Colorado"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 7
                        }, 
                        {
                            "name": "l", 
                            "value": 8
                        }, 
                        {
                            "name": "gf", 
                            "value": 53
                        }, 
                        {
                            "name": "ga", 
                            "value": 66
                        }, 
                        {
                            "name": "gd", 
                            "value": -13
                        }, 
                        {
                            "name": "pts", 
                            "value": 18
                        }
                    ], 
                    "team": {
                        "id": 28058, 
                        "link": "http://www.everysport.com/sport/ishockey/team/calgary-flames/28058", 
                        "name": "Calgary Flames", 
                        "shortName": "Calgary"
                    }
                }
            ]
        }, 
        {
            "labels": [
                {
                    "name": "Western Conference", 
                    "type": "conference"
                }, 
                {
                    "name": "Pacific Division", 
                    "type": "division"
                }
            ], 
            "standings": [
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 18
                        }, 
                        {
                            "name": "w", 
                            "value": 14
                        }, 
                        {
                            "name": "l", 
                            "value": 3
                        }, 
                        {
                            "name": "gf", 
                            "value": 64
                        }, 
                        {
                            "name": "ga", 
                            "value": 48
                        }, 
                        {
                            "name": "gd", 
                            "value": 16
                        }, 
                        {
                            "name": "pts", 
                            "value": 29
                        }
                    ], 
                    "team": {
                        "id": 28076, 
                        "link": "http://www.everysport.com/sport/ishockey/team/anaheim-ducks/28076", 
                        "name": "Anaheim Ducks", 
                        "shortName": "Anaheim"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 18
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 6
                        }, 
                        {
                            "name": "gf", 
                            "value": 47
                        }, 
                        {
                            "name": "ga", 
                            "value": 42
                        }, 
                        {
                            "name": "gd", 
                            "value": 5
                        }, 
                        {
                            "name": "pts", 
                            "value": 22
                        }
                    ], 
                    "team": {
                        "id": 28060, 
                        "link": "http://www.everysport.com/sport/ishockey/team/los-angeles-kings/28060", 
                        "name": "Los Angeles Kings", 
                        "shortName": "Los Angeles"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 21
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 9
                        }, 
                        {
                            "name": "gf", 
                            "value": 57
                        }, 
                        {
                            "name": "ga", 
                            "value": 62
                        }, 
                        {
                            "name": "gd", 
                            "value": -5
                        }, 
                        {
                            "name": "pts", 
                            "value": 22
                        }
                    ], 
                    "team": {
                        "id": 28059, 
                        "link": "http://www.everysport.com/sport/ishockey/team/dallas-stars/28059", 
                        "name": "Dallas Stars", 
                        "shortName": "Dallas"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 9
                        }, 
                        {
                            "name": "l", 
                            "value": 6
                        }, 
                        {
                            "name": "gf", 
                            "value": 45
                        }, 
                        {
                            "name": "ga", 
                            "value": 43
                        }, 
                        {
                            "name": "gd", 
                            "value": 2
                        }, 
                        {
                            "name": "pts", 
                            "value": 22
                        }
                    ], 
                    "team": {
                        "id": 28068, 
                        "link": "http://www.everysport.com/sport/ishockey/team/san-jose-sharks/28068", 
                        "name": "San Jose Sharks", 
                        "shortName": "San Jose"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 9
                        }, 
                        {
                            "name": "l", 
                            "value": 8
                        }, 
                        {
                            "name": "gf", 
                            "value": 57
                        }, 
                        {
                            "name": "ga", 
                            "value": 55
                        }, 
                        {
                            "name": "gd", 
                            "value": 2
                        }, 
                        {
                            "name": "pts", 
                            "value": 21
                        }
                    ], 
                    "team": {
                        "id": 28064, 
                        "link": "http://www.everysport.com/sport/ishockey/team/phoenix-coyotes/28064", 
                        "name": "Phoenix Coyotes", 
                        "shortName": "Phoenix"
                    }
                }
            ]
        }, 
        {
            "labels": [
                {
                    "name": "Eastern Conference", 
                    "type": "conference"
                }, 
                {
                    "name": "Atlantic Division", 
                    "type": "division"
                }
            ], 
            "standings": [
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 21
                        }, 
                        {
                            "name": "w", 
                            "value": 13
                        }, 
                        {
                            "name": "l", 
                            "value": 8
                        }, 
                        {
                            "name": "gf", 
                            "value": 70
                        }, 
                        {
                            "name": "ga", 
                            "value": 58
                        }, 
                        {
                            "name": "gd", 
                            "value": 12
                        }, 
                        {
                            "name": "pts", 
                            "value": 26
                        }
                    ], 
                    "team": {
                        "id": 28062, 
                        "link": "http://www.everysport.com/sport/ishockey/team/pittsburgh-penguins/28062", 
                        "name": "Pittsburgh Penguins", 
                        "shortName": "Pittsburgh"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 6
                        }, 
                        {
                            "name": "gf", 
                            "value": 49
                        }, 
                        {
                            "name": "ga", 
                            "value": 52
                        }, 
                        {
                            "name": "gd", 
                            "value": -3
                        }, 
                        {
                            "name": "pts", 
                            "value": 24
                        }
                    ], 
                    "team": {
                        "id": 28061, 
                        "link": "http://www.everysport.com/sport/ishockey/team/new-jersey-devils/28061", 
                        "name": "New Jersey Devils", 
                        "shortName": "New Jersey"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 22
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 11
                        }, 
                        {
                            "name": "gf", 
                            "value": 64
                        }, 
                        {
                            "name": "ga", 
                            "value": 67
                        }, 
                        {
                            "name": "gd", 
                            "value": -3
                        }, 
                        {
                            "name": "pts", 
                            "value": 21
                        }
                    ], 
                    "team": {
                        "id": 28069, 
                        "link": "http://www.everysport.com/sport/ishockey/team/philadelphia-flyers/28069", 
                        "name": "Philadelphia Flyers", 
                        "shortName": "Philadelphia"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 9
                        }, 
                        {
                            "name": "l", 
                            "value": 8
                        }, 
                        {
                            "name": "gf", 
                            "value": 48
                        }, 
                        {
                            "name": "ga", 
                            "value": 49
                        }, 
                        {
                            "name": "gd", 
                            "value": -1
                        }, 
                        {
                            "name": "pts", 
                            "value": 20
                        }
                    ], 
                    "team": {
                        "id": 28070, 
                        "link": "http://www.everysport.com/sport/ishockey/team/new-york-rangers/28070", 
                        "name": "New York Rangers", 
                        "shortName": "NY Rangers"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 21
                        }, 
                        {
                            "name": "w", 
                            "value": 8
                        }, 
                        {
                            "name": "l", 
                            "value": 11
                        }, 
                        {
                            "name": "gf", 
                            "value": 61
                        }, 
                        {
                            "name": "ga", 
                            "value": 73
                        }, 
                        {
                            "name": "gd", 
                            "value": -12
                        }, 
                        {
                            "name": "pts", 
                            "value": 18
                        }
                    ], 
                    "team": {
                        "id": 28052, 
                        "link": "http://www.everysport.com/sport/ishockey/team/new-york-islanders/28052", 
                        "name": "New York Islanders", 
                        "shortName": "NY Islanders"
                    }
                }
            ]
        }, 
        {
            "labels": [
                {
                    "name": "Eastern Conference", 
                    "type": "conference"
                }, 
                {
                    "name": "Northeast Division", 
                    "type": "division"
                }
            ], 
            "standings": [
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 13
                        }, 
                        {
                            "name": "l", 
                            "value": 4
                        }, 
                        {
                            "name": "gf", 
                            "value": 58
                        }, 
                        {
                            "name": "ga", 
                            "value": 43
                        }, 
                        {
                            "name": "gd", 
                            "value": 15
                        }, 
                        {
                            "name": "pts", 
                            "value": 29
                        }
                    ], 
                    "team": {
                        "id": 28066, 
                        "link": "http://www.everysport.com/sport/ishockey/team/montreal-canadiens/28066", 
                        "name": "Montreal Canadiens", 
                        "shortName": "Montreal"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 17
                        }, 
                        {
                            "name": "w", 
                            "value": 13
                        }, 
                        {
                            "name": "l", 
                            "value": 2
                        }, 
                        {
                            "name": "gf", 
                            "value": 51
                        }, 
                        {
                            "name": "ga", 
                            "value": 36
                        }, 
                        {
                            "name": "gd", 
                            "value": 15
                        }, 
                        {
                            "name": "pts", 
                            "value": 28
                        }
                    ], 
                    "team": {
                        "id": 28065, 
                        "link": "http://www.everysport.com/sport/ishockey/team/boston-bruins/28065", 
                        "name": "Boston Bruins", 
                        "shortName": "Boston"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 21
                        }, 
                        {
                            "name": "w", 
                            "value": 12
                        }, 
                        {
                            "name": "l", 
                            "value": 6
                        }, 
                        {
                            "name": "gf", 
                            "value": 49
                        }, 
                        {
                            "name": "ga", 
                            "value": 39
                        }, 
                        {
                            "name": "gd", 
                            "value": 10
                        }, 
                        {
                            "name": "pts", 
                            "value": 27
                        }
                    ], 
                    "team": {
                        "id": 28050, 
                        "link": "http://www.everysport.com/sport/ishockey/team/ottawa-senators/28050", 
                        "name": "Ottawa Senators", 
                        "shortName": "Ottawa"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 22
                        }, 
                        {
                            "name": "w", 
                            "value": 13
                        }, 
                        {
                            "name": "l", 
                            "value": 9
                        }, 
                        {
                            "name": "gf", 
                            "value": 64
                        }, 
                        {
                            "name": "ga", 
                            "value": 55
                        }, 
                        {
                            "name": "gd", 
                            "value": 9
                        }, 
                        {
                            "name": "pts", 
                            "value": 26
                        }
                    ], 
                    "team": {
                        "id": 28049, 
                        "link": "http://www.everysport.com/sport/ishockey/team/toronto-maple-leafs/28049", 
                        "name": "Toronto Maple Leafs", 
                        "shortName": "Toronto"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 21
                        }, 
                        {
                            "name": "w", 
                            "value": 8
                        }, 
                        {
                            "name": "l", 
                            "value": 12
                        }, 
                        {
                            "name": "gf", 
                            "value": 54
                        }, 
                        {
                            "name": "ga", 
                            "value": 67
                        }, 
                        {
                            "name": "gd", 
                            "value": -13
                        }, 
                        {
                            "name": "pts", 
                            "value": 17
                        }
                    ], 
                    "team": {
                        "id": 28051, 
                        "link": "http://www.everysport.com/sport/ishockey/team/buffalo-sabres/28051", 
                        "name": "Buffalo Sabres", 
                        "shortName": "Buffalo"
                    }
                }
            ]
        }, 
        {
            "labels": [
                {
                    "name": "Eastern Conference", 
                    "type": "conference"
                }, 
                {
                    "name": "Southeast Division", 
                    "type": "division"
                }
            ], 
            "standings": [
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 8
                        }, 
                        {
                            "name": "gf", 
                            "value": 54
                        }, 
                        {
                            "name": "ga", 
                            "value": 55
                        }, 
                        {
                            "name": "gd", 
                            "value": -1
                        }, 
                        {
                            "name": "pts", 
                            "value": 21
                        }
                    ], 
                    "team": {
                        "id": 28056, 
                        "link": "http://www.everysport.com/sport/ishockey/team/carolina-hurricanes/28056", 
                        "name": "Carolina Hurricanes", 
                        "shortName": "Carolina"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 10
                        }, 
                        {
                            "name": "l", 
                            "value": 9
                        }, 
                        {
                            "name": "gf", 
                            "value": 55
                        }, 
                        {
                            "name": "ga", 
                            "value": 61
                        }, 
                        {
                            "name": "gd", 
                            "value": -6
                        }, 
                        {
                            "name": "pts", 
                            "value": 21
                        }
                    ], 
                    "team": {
                        "id": 109005, 
                        "link": "http://www.everysport.com/sport/ishockey/team/winnipeg-jets/109005", 
                        "name": "Winnipeg Jets", 
                        "shortName": "Winnipeg"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 9
                        }, 
                        {
                            "name": "l", 
                            "value": 10
                        }, 
                        {
                            "name": "gf", 
                            "value": 71
                        }, 
                        {
                            "name": "ga", 
                            "value": 64
                        }, 
                        {
                            "name": "gd", 
                            "value": 7
                        }, 
                        {
                            "name": "pts", 
                            "value": 19
                        }
                    ], 
                    "team": {
                        "id": 28055, 
                        "link": "http://www.everysport.com/sport/ishockey/team/tampa-bay-lightning/28055", 
                        "name": "Tampa Bay Lightning", 
                        "shortName": "Tampa Bay"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 20
                        }, 
                        {
                            "name": "w", 
                            "value": 6
                        }, 
                        {
                            "name": "l", 
                            "value": 9
                        }, 
                        {
                            "name": "gf", 
                            "value": 51
                        }, 
                        {
                            "name": "ga", 
                            "value": 73
                        }, 
                        {
                            "name": "gd", 
                            "value": -22
                        }, 
                        {
                            "name": "pts", 
                            "value": 17
                        }
                    ], 
                    "team": {
                        "id": 28047, 
                        "link": "http://www.everysport.com/sport/ishockey/team/florida-panthers/28047", 
                        "name": "Florida Panthers", 
                        "shortName": "Florida"
                    }
                }, 
                {
                    "stats": [
                        {
                            "name": "gp", 
                            "value": 19
                        }, 
                        {
                            "name": "w", 
                            "value": 7
                        }, 
                        {
                            "name": "l", 
                            "value": 11
                        }, 
                        {
                            "name": "gf", 
                            "value": 52
                        }, 
                        {
                            "name": "ga", 
                            "value": 59
                        }, 
                        {
                            "name": "gd", 
                            "value": -7
                        }, 
                        {
                            "name": "pts", 
                            "value": 15
                        }
                    ], 
                    "team": {
                        "id": 28073, 
                        "link": "http://www.everysport.com/sport/ishockey/team/washington-capitals/28073", 
                        "name": "Washington Capitals", 
                        "shortName": "Washington"
                    }
                }
            ]
        }
    ]
}
```


	
        	
