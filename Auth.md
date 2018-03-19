# chatserver_docs
All docs and design specs for our client-server based chat application to rule the world!

## AUTHENTIFICATION METHOD
```csharp

private string UserName = "";  // Nickname
private string Status = ""; // online, away, offline >> maybe realized with State Pattern?
private string clientipAddress = "0.0.0.0"; // Client IP Adress
private string sessionId; // PC-Name = Console.WriteLine("MachineName: {0}", Environment.MachineName);
private string password = "12345"; // The password
```

## Description

The password and username and/or connectID shoud be stored in a database at first connection.
In any further connection the credentials will be checked with database entry.


## Example JSON Code

```json
{
  "from": "127.0.01.",
  "to": ["benutzername", "#channel"],
  "msg": "{
    "userName":"Test",
    "status":"offline",
    "sessionId": "pcname",
    "password":"A12345"
  }",
  "method": "auth",
  "createdAt": "Datetime"
}
```

