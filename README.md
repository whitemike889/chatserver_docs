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

* `from` lists the nickname from the sender
* `to` Array of strings, contains the desired users/channel this message should be routed to. Channels start with a `#`
* `msg` generic string which contains the actual payload. For example the message that we want to send to another user
* `methods` This is an enum. Allowed values are the methods listed below. This field is case sensitive
* `createdAt` Datetime. Determines the creation time of the json object

## Methods

* [getUsers](getusers.md)
* getChannels
* auth
* [getUserDetails](getuserdetails.md)
* [chat](chat.md)