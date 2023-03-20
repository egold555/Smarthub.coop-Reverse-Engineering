# User Profile Request
Returns information about the user profile
```
Method: GET
URL: https://elmhurstmutual.smarthub.coop/services/secured/userProfile?emailAddress=email%40gmail.com
Requires Auth: Yes
```

## Request Parameters:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  emailAddress   |   Email address of your account  |


## Response:
```json
{
  "domain": "elmhurstmutual",
  "emailAddress": "REDACTED",
  "registeredOn": 1675272129973,
  "firstLogin": 1675272130689,
  "paperBillsActionRequired": true,
  "lastSuccessfulLogin": 1678322641414,
  "lastViewedCustomPromptVersion": 0,
  "lastViewedCustomPromptVersionMobile": 0,
  "termTypesRequiringApproval": [
    "VOICE_NOTIFICATIONS",
    "TEXT_NOTIFICATIONS",
    "EMAIL_NOTIFICATIONS",
    "DO_NOT_CALL"
  ],
  "acceptedTerms": [
    {
      "termType": "AUTO_PAY",
      "termMajorVersionAccepted": 1,
      "termMinorVersionAccepted": 0,
      "termAcceptDate": 1675276135519,
      "ipAddress": "REDACTED",
      "browserUserAgent": "REDACTED"
    }
  ]
}
```