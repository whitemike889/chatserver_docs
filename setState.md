# setState Method

## Example for Method Call and new Enumeration:

```
enum userState {ONLINE, OFFLINE, OCCUPIED, INVISIBLE};
setState(userState state)
```

The method triggers an small update for the database like
`"UPDATE user SET state = " + state.toString() + " WHERE userId = " + userId;`

## Description of states

OFFLINE triggers `disconnect` and quits the connection.
ONLINE, OCCUPIED, INVISIBLE triggers `connect` when not connected and establish a new connection.
OCCUPIED will be the same as ONLINE but can be displayed another way.
INVISIBLE will always answer with OFFLINE, but the user can write into his channels.

## Expected JSON

```JSON
{
  "from": "String",
  "to": ["String"],
  "msg": "INVISIBLE",
  "method": "setState",
  "createdAt": "Datetime"
}
```
