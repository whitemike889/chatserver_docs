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

* GetUsers
* GetChannel
* Auth
[* GetUserDetails](https://github.com/TI114/chatserver_docs/blob/getUserDetails/getuserdetails.md)

### AUTH Methodendefinition
```c# 

private string UserName = "";  
private string Status = ""; // online, offline usw
private string ipAddress = "0.0.0.0"; // Client IP
private string connectId; // PC-Name = Console.WriteLine("MachineName: {0}", Environment.MachineName);

```
