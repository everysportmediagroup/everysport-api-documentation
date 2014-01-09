# Live Score API

All ongoing events is returned with a status of 'ongoing'. To get the current ongoing events a GET-request is performed against the events collection `GET /events` and all events that match the query is returned in the response.

Example: If you want to get all the ongoing football events for today you perform the following query:  
`GET /events?sport=10&fromDate=2014-01-09&toDate=2014-01-09&status=ongoing`

It is necessary to handle the logic in the client for when an event switches from ongoing to finished.
