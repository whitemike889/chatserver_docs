# chat command

## Purpose

This command is the core functionality of the application. We want to send
strings from one client to another one (or several).

### Client to Server

```json
{
  "from": "String",
  "to": ["String"],
  "msg": "String",
  "method": "String",
  "createdAt": "Datetime",
}
```

* `from` field contains the local username
* `to` field is an array. it contains one entry for each receiver. Receiver
starting with a `#` are channels/chatrooms.
* `msg` this is the text that we want to send from one client to another
* `createdAt` Datetime from the message creation

### Server to client

This is the same payload as above.

* `from` contains the name from the sender
* `to` contains an array with one element, the name of the receiver
