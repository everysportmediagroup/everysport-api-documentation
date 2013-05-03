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
* round - specifies standings after a specific round, eg. '10'. Default is the last played round.
* size - specifies the amount of statistics data for the teams. Default is 'large' which retrieves all available data. Use  'medium' and 'small' to get less data. 
* sort - the key by which the standings is sorted. Can be any of the attribute names from the Team Stats objects (eg. 'stats.pts') or 'team.name' to sort by the name of the team. By default, sorting is by 'stats.pts'.   
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 


## Example Request

	GET http://api.everysport.com/v1/leagues/58878/standings


```javascript	
{
    credit: {
        message: "Provided by Everysport.com",
            link: "http://www.everysport.com",
            logoUrl: "http://c.static.es-cdn.net/files/everysport2/images/icons/event/small/everysport.png"
    },
    metadata: { },
    groups: [
        {
            labels: [ ],
            standings: [
                {
                    team: {
                        id: 9370,
                        name: "IFK Göteborg",
                        shortName: "Göteborg",
                        link: "http://www.everysport.com/sport/fotboll/team/ifk-goeteborg/9370"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 4
                        },
                        {
                            name: "d",
                            value: 1
                        },
                        {
                            name: "l",
                            value: 0
                        },
                        {
                            name: "gf",
                            value: 9
                        },
                        {
                            name: "ga",
                            value: 1
                        },
                        {
                            name: "gd",
                            value: 8
                        },
                        {
                            name: "pts",
                            value: 13
                        }
                    ]
                },
                {
                    team: {
                        id: 9375,
                        name: "Malmö FF",
                        shortName: "Malmö FF",
                        link: "http://www.everysport.com/sport/fotboll/team/malmoe-ff/9375"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 4
                        },
                        {
                            name: "d",
                            value: 1
                        },
                        {
                            name: "l",
                            value: 0
                        },
                        {
                            name: "gf",
                            value: 8
                        },
                        {
                            name: "ga",
                            value: 2
                        },
                        {
                            name: "gd",
                            value: 6
                        },
                        {
                            name: "pts",
                            value: 13
                        }
                    ]
                },
                {
                    team: {
                        id: 9373,
                        name: "Helsingborgs IF",
                        shortName: "Helsingborg",
                        link: "http://www.everysport.com/sport/fotboll/team/helsingborgs-if/9373"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 3
                        },
                        {
                            name: "d",
                            value: 1
                        },
                        {
                            name: "l",
                            value: 1
                        },
                        {
                            name: "gf",
                            value: 11
                        },
                        {
                            name: "ga",
                            value: 4
                        },
                        {
                            name: "gd",
                            value: 7
                        },
                        {
                            name: "pts",
                            value: 10
                        }
                    ]
                },
                {
                    team: {
                        id: 9374,
                        name: "Kalmar FF",
                        shortName: "Kalmar FF",
                        link: "http://www.everysport.com/sport/fotboll/team/kalmar-ff/9374"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 2
                        },
                        {
                            name: "d",
                            value: 2
                        },
                        {
                            name: "l",
                            value: 1
                        },
                        {
                            name: "gf",
                            value: 6
                        },
                        {
                            name: "ga",
                            value: 3
                        },
                        {
                            name: "gd",
                            value: 3
                        },
                        {
                            name: "pts",
                            value: 8
                        }
                    ]
                },
                {
                    team: {
                        id: 9394,
                        name: "Östers IF",
                        shortName: "Öster",
                        link: "http://www.everysport.com/sport/fotboll/team/oesters-if/9394"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 2
                        },
                        {
                            name: "d",
                            value: 2
                        },
                        {
                            name: "l",
                            value: 1
                        },
                        {
                            name: "gf",
                            value: 6
                        },
                        {
                            name: "ga",
                            value: 5
                        },
                        {
                            name: "gd",
                            value: 1
                        },
                        {
                            name: "pts",
                            value: 8
                        }
                    ]
                },
                {
                    team: {
                        id: 9369,
                        name: "IF Elfsborg",
                        shortName: "Elfsborg",
                        link: "http://www.everysport.com/sport/fotboll/team/if-elfsborg/9369"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 1
                        },
                        {
                            name: "d",
                            value: 4
                        },
                        {
                            name: "l",
                            value: 0
                        },
                        {
                            name: "gf",
                            value: 6
                        },
                        {
                            name: "ga",
                            value: 4
                        },
                        {
                            name: "gd",
                            value: 2
                        },
                        {
                            name: "pts",
                            value: 7
                        }
                    ]
                },
                {
                    team: {
                        id: 19740,
                        name: "BK Häcken",
                        shortName: "Häcken",
                        link: "http://www.everysport.com/sport/fotboll/team/bk-haecken/19740"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 2
                        },
                        {
                            name: "d",
                            value: 1
                        },
                        {
                            name: "l",
                            value: 2
                        },
                        {
                            name: "gf",
                            value: 6
                        },
                        {
                            name: "ga",
                            value: 5
                        },
                        {
                            name: "gd",
                            value: 1
                        },
                        {
                            name: "pts",
                            value: 7
                        }
                    ]
                },
                {
                    team: {
                        id: 9400,
                        name: "Gefle IF",
                        shortName: "Gefle",
                        link: "http://www.everysport.com/sport/fotboll/team/gefle-if/9400"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 2
                        },
                        {
                            name: "d",
                            value: 0
                        },
                        {
                            name: "l",
                            value: 3
                        },
                        {
                            name: "gf",
                            value: 5
                        },
                        {
                            name: "ga",
                            value: 5
                        },
                        {
                            name: "gd",
                            value: 0
                        },
                        {
                            name: "pts",
                            value: 6
                        }
                    ]
                },
                {
                    team: {
                        id: 9389,
                        name: "Mjällby AIF",
                        shortName: "Mjällby",
                        link: "http://www.everysport.com/sport/fotboll/team/mjaellby-aif/9389"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 4
                        },
                        {
                            name: "w",
                            value: 2
                        },
                        {
                            name: "d",
                            value: 0
                        },
                        {
                            name: "l",
                            value: 2
                        },
                        {
                            name: "gf",
                            value: 4
                        },
                        {
                            name: "ga",
                            value: 5
                        },
                        {
                            name: "gd",
                            value: -1
                        },
                        {
                            name: "pts",
                            value: 6
                        }
                    ]
                },
                {
                    team: {
                        id: 9376,
                        name: "IFK Norrköping",
                        shortName: "Norrköping",
                        link: "http://www.everysport.com/sport/fotboll/team/ifk-norrkoeping/9376"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 2
                        },
                        {
                            name: "d",
                            value: 0
                        },
                        {
                            name: "l",
                            value: 3
                        },
                        {
                            name: "gf",
                            value: 6
                        },
                        {
                            name: "ga",
                            value: 10
                        },
                        {
                            name: "gd",
                            value: -4
                        },
                        {
                            name: "pts",
                            value: 6
                        }
                    ]
                },
                {
                    team: {
                        id: 9367,
                        name: "AIK",
                        shortName: "AIK",
                        link: "http://www.everysport.com/sport/fotboll/team/aik/9367"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 1
                        },
                        {
                            name: "d",
                            value: 2
                        },
                        {
                            name: "l",
                            value: 2
                        },
                        {
                            name: "gf",
                            value: 4
                        },
                        {
                            name: "ga",
                            value: 5
                        },
                        {
                            name: "gd",
                            value: -1
                        },
                        {
                            name: "pts",
                            value: 5
                        }
                    ]
                },
                {
                    team: {
                        id: 19721,
                        name: "IF Brommapojkarna",
                        shortName: "Brommapojkarna",
                        link: "http://www.everysport.com/sport/fotboll/team/if-brommapojkarna/19721"
                    },
                    positionStatuses: [ ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 1
                        },
                        {
                            name: "d",
                            value: 2
                        },
                        {
                            name: "l",
                            value: 2
                        },
                        {
                            name: "gf",
                            value: 4
                        },
                        {
                            name: "ga",
                            value: 7
                        },
                        {
                            name: "gd",
                            value: -3
                        },
                        {
                            name: "pts",
                            value: 5
                        }
                    ]
                },
                {
                    team: {
                        id: 9393,
                        name: "Åtvidabergs FF",
                        shortName: "Åtvidaberg",
                        link: "http://www.everysport.com/sport/fotboll/team/aatvidabergs-ff/9393"
                    },
                    positionStatuses: [ ],
                    lineThicknessBelow: 1,
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 1
                        },
                        {
                            name: "d",
                            value: 1
                        },
                        {
                            name: "l",
                            value: 3
                        },
                        {
                            name: "gf",
                            value: 3
                        },
                        {
                            name: "ga",
                            value: 6
                        },
                        {
                            name: "gd",
                            value: -3
                        },
                        {
                            name: "pts",
                            value: 4
                        }
                    ]
                },
                {
                    team: {
                        id: 23026,
                        name: "Syrianska FC",
                        shortName: "Syrianska",
                        link: "http://www.everysport.com/sport/fotboll/team/syrianska-fc/23026"
                    },
                    positionStatuses: [
                        {
                            type: "negative-qualifying",
                            name: "Negativt kval"
                        }
                    ],
                    lineThicknessBelow: 2,
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 1
                        },
                        {
                            name: "d",
                            value: 1
                        },
                        {
                            name: "l",
                            value: 3
                        },
                        {
                            name: "gf",
                            value: 3
                        },
                        {
                            name: "ga",
                            value: 7
                        },
                        {
                            name: "gd",
                            value: -4
                        },
                        {
                            name: "pts",
                            value: 4
                        }
                    ]
                },
                {
                    team: {
                        id: 9371,
                        name: "Halmstads BK",
                        shortName: "Halmstad",
                        link: "http://www.everysport.com/sport/fotboll/team/halmstads-bk/9371"
                    },
                    positionStatuses: [
                        {
                            type: "relegation",
                            name: "Nedflyttning"
                        }
                    ],
                    stats: [
                        {
                            name: "gp",
                            value: 5
                        },
                        {
                            name: "w",
                            value: 0
                        },
                        {
                            name: "d",
                            value: 3
                        },
                        {
                            name: "l",
                            value: 2
                        },
                        {
                            name: "gf",
                            value: 3
                        },
                        {
                            name: "ga",
                            value: 6
                        },
                        {
                            name: "gd",
                            value: -3
                        },
                        {
                            name: "pts",
                            value: 3
                        }
                    ]
                },
                {
                    team: {
                        id: 9368,
                        name: "Djurgårdens IF FF",
                        shortName: "Djurgården",
                        link: "http://www.everysport.com/sport/fotboll/team/djurgaardens-if-ff/9368"
                    },
                    positionStatuses: [
                        {
                            type: "relegation",
                            name: "Nedflyttning"
                        }
                    ],
                    stats: [
                        {
                            name: "gp",
                            value: 4
                        },
                        {
                            name: "w",
                            value: 0
                        },
                        {
                            name: "d",
                            value: 1
                        },
                        {
                            name: "l",
                            value: 3
                        },
                        {
                            name: "gf",
                            value: 1
                        },
                        {
                            name: "ga",
                            value: 10
                        },
                        {
                            name: "gd",
                            value: -9
                        },
                        {
                            name: "pts",
                            value: 1
                        }
                    ]
                }
            ]
        }
    ]
}
```


	
        	
