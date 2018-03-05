# GetUser Method
Define GetUser Method in server application

## Ideas, which type of result we need

Get the list of the users with a Tlist Object.

This will be an export from the database with a select statement in the backend.

We need an unique userid, to identify the user correctly.

We also need a result for each channel. A count from each Group will be fine.

## examples, which result i think what we need

```JSON
	{
		"UserID" : "integer",
		"UserName" : "string",
		"FirstName" : "string",
		"LastName" : "string",
		"ConnectionID" : "integer",

	}
```
```JSON
	{
		"UserID" : "integer",
    		"ChannelID" : "integer",
    		"ConnectionID" : "integer",
	}
		
```
