# Standings

    GET leagues/:id/standings

## Description
Returns a list of the current standings (i.e. the Table) for the league. 

## Parameters
* id (required) - The League ID
* type - one of 'total' (default), 'home' and 'away' 
* callback - used for JSON-P callbacks, the argument should be the name of the callback function, such as 'esResults' 

## Return format
An object with the following keys and values:
* credits - a Credits object
* standings - a list of Team Standings objects, one for each team in the league 

Each Standings object contains the following data: 
* team - a Team object in short form
* stats - a Team Stats object







 