# Standings

    GET leagues/:id/standings

## Description
Returns a list of the current standings (i.e. the Table) for the league. 

## Parameters
* id (required) - The League ID
* type - one of 'total' (default), 'home' and 'away' 
* sortKey - the key by which the standings is sorted. Can be any of the attribute names from the Team Stats objects (eg. 'stats.pts') or 'team.name' to sort by the name of the team. By default, sorting is by 'stats.pts'.   
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 

## Return format
An object with the following keys and values:
* credits - a Credits object
* groups - a list of one or many Groups objects. For example, in NHL one group is the "Western Conference" and another is "Atlantic Division". One team may belong to more than one group.  

### Group object
A Group object has the following data: 
* name - the name of the group, string
* standings - a list of Standings objects

### Standings object
A Standings object has the following data: 
* team - a Team Object in short format
* stats - a Team Stats Object  








 