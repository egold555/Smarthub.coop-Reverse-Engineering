# Push Notification Registry Request
Register a device for push notifications
```
Method: POST
URL: /services/secured/device/pushRegistration
Requires Auth: Yes or No
```
## Additional Headers:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  content-type   |  application/json;   |



## Post Body:
```json
{
  "deviceRegistration": {
    "application": "SmartHub",
    "applicationId": "coop.nisc.android.smarthub",
    "device": {
      "alias": "samsung SM-G950U",
      "id": "REDACTED",
      "type": "ANDROID"
    }
  },
  "pushToken": "REDACTED"
}

```

## Response:
```json
{
  "deviceRegistration": {
    "device": {
      "id": "REDACTED",
      "alias": "samsung SM-G950U",
      "type": "ANDROID"
    },
    "application": "SmartHub",
    "applicationId": "coop.nisc.android.smarthub"
  },
  "pushToken": "REDACTED",
  "pushRegistrationStatus": "REGISTERED"
}
```

## Misc Notes:
Unsure how pushToken is generated?
https://developers.google.com/resources/api-libraries/documentation/games/v1/java/latest/com/google/api/services/games/model/PushToken.html