# Events

    GET leagues/:id/events

## Description
Returns a list of Event objects for the league.

## Parameters
* id (required) - the League ID
* status - one of 'upcoming','ongoing','finished', 'postponed', 'interrupted', 'all'(default)
* fromDate - filters out events after a specific date, Date in short format
* to date - filters out events before a specific date, Date in short format
* limit - Limits the number of events, positive integer

## Return format
An object with the following keys and values:
* credits - a Credit object
* events - a list of Event objects
