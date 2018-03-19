# chatserver_docs
All docs and design specs for our client-server based chat application to rule the world!

## JSON schema for generic messages

```json
{
  "from": "String",
  "to": ["String"],
  "msg": "String",
  "method": "String",
  "createdAt": "Datetime",
}
```

## Methods

* [getUsers](getusers.md)
* getChannels
* auth
* [getUserDetails](getuserdetails.md)
* [chat](chat.md)