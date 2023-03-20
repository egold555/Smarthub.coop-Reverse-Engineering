# NAME Request
```
Method: GET
URL: https://elmhurstmutual.smarthub.coop/services/memberLookup/domain?domain=elmhurstmutual
Requires Auth: No
```

## Request Parameters:
| Key             | Value                                                |
| --------------- | -----------------------------------------------------|
| domain          | Domain from [Search Request]()                       |

## Response:
```json
[
  {
    "domain": "elmhurstmutual",
    "name": "Elmhurst Mutual Power and Light",
    "addressList": [
      {
        "name": "Elmhurst Power",
        "addressType": "HQ",
        "addressLine1": "120 132nd Street",
        "addressLine2": "",
        "city": "Tacoma",
        "state": "WA",
        "zip": "98444",
        "latitude": 47.136929,
        "longitude": -122.433512
      }
    ],
    "registrationInformation": {
      "ssnRequired": false,
      "registerDoNotAllow": false,
      "registrationNotAllowedMessage": "Your account does not have the information required to verify your identity online.  Please contact customer service during normal business hours at (253) 531-4646.",
      "securityQuestionsListBox": "BILL,BILLING_ZIP,ZIP",
      "minimumPasswordLength": 6,
      "maximumPasswordLength": 15,
      "registrationConfirmationScreenTitle": "Congratulations!",
      "registrationConfirmationMessage": "Your registration is complete. You will receive an email with instructions for setting your password.",
      "numberOfSecurityQuestionsRequired": 1,
      "minimumPasswordNumericCharacters": 1,
      "minimumPasswordSpecialCharacters": 0,
      "minimumPasswordUppercaseCharacters": 1,
      "lostCredentialsSecurityQuestionsListBox": "BILL,BILLING_ZIP,ZIP",
      "lostCredentialsNumberOfSecurityQuestionsRequired": 1,
      "requireAccountNumberOnPasswordReset": true,
      "hintQuestionsToPrompt": 3,
      "cpniPasswordLabel": "CPNI Password",
      "failedLoginLockoutLimit": 5
    },
    "imageResource": "https://elmhurstmutual.smarthub.coop/services/themes/resources?resource=smarthub-login-grn.jpg",
    "availableSystems": [
      "ABS",
      "AMS",
      "CIS",
      "OMS",
      "MDM"
    ],
    "minVersion": 10,
    "consumerGlobalInformation": {
      "lockoutMessage": "Invalid login. Repeated failed login attempts will lock your account. ",
      "offlineMessage": "SmartHub is currently offline. <br>Please try again later.",
      "telecomIndustryKeyword": "",
      "utilityIndustryKeyword": ""
    },
    "primaryColor": "#316bbc",
    "primaryTextColor": "#FFFFFF",
    "smarthubWifiEnabled": false
  }
]
```

## Misc Notes:
Any notes here