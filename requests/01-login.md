# Login Request
Login request to get a session token.
```
Method: Post
URL: https://elmhurstmutual.smarthub.coop/services/user-login/authenticate
Requires Auth: No
```

## Additional Headers:
| Key             | Value                              |
| --------------- | -----------------------------------|
| content-type    | application/json; charset=utf-8    |

## Post Body:
```json
// MINIFIED when submitting
{
  "password": "PASSWORD_AS_PLAIN_TEXT",
  "rememberMe": false,
  "rememberTwoFactorAuth": false,
  "twoFactorCode": "",
  "username": "email@gmail.com"
}
```
## Response Headers:
```
JSESSIONID-consumer_13.13.6=REDACTTED; Path=/; Secure; HttpOnly; SameSite=None
XSRF-TOKEN=REDACTED; Path=/; Secure; SameSite=None
```

## Success Response:
```json
{
  "status": "SUCCESS",
  "userDetails": {
    "id": "email@gmail.com",
    "name": "ERIC GOLDE",
    "paperBills": false,
    "emailNotifications": true,
    "serviceLocations": [
      {
        "accountNumber": "--REDACTED--",
        "serviceLocation": "--REDACTED--"
      }
    ],
    "userGroups": [],
    "memberIds": [],
    "memberInformation": []
  }
}
```
## Failure Response:
```json
{
  "status": "FAILURE"
}
```

## Misc Notes:
This request response of session tokens doesn't seem to be used.

All subsequent requests use the `Authorizatio Basic` header, described in the [Authentication & Headers](requests/00-../00-authorization-and-headers.md) file.

I can make requests without calling this endpoint, but I'm unsure why it would be implemented like this, or if I am missing something here.