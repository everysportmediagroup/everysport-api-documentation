# Standings

>    GET leagues/:id/standings

## Description
Returns a list of the current standing (aka The Table) for each team in the league. 

## Parameters
* id (required) - The League ID from everysport.com
* type - one of 'total' (default), 'home' and 'away'. 

## Return format
An object with the following keys and values:
* credits
* standings - a list of Team objects
* meta




 