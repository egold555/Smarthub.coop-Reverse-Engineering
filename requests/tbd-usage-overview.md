# NAME Request
Short description of the request
```
Method: GET
URL: /services/secured/usage-overview/ACCOUNT_NUMBER/SERVICE_LOCATION/ELECTRIC
Requires Auth: Yes
```

## Request Parameters:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  ACCOUNT_NUMBER |  Found in the [user login](01-login.md)   |
|  SERVICE_LOCATION |  Found in the [user login](01-login.md)   |

## Response:
```json
{
  "customer": "REDACTED",
  "account": "REDACTED",
  "serviceLocation": "REDACTED",
  "industry": "ELECTRIC",
  "providers": [
    "ELM"
  ],
  "services": [
    "ELEC"
  ],
  "displayMode": "PRICE",
  "current": {
    "month": 2,
    "year": 2023,
    "usage": 198,
    "cost": 49,
    "unitsOfMeasure": [
      "KWH"
    ]
  },
  "pastYearOverviewData": [
    {
      "month": 2,
      "year": 2023,
      "usage": 198,
      "cost": 49,
      "unitsOfMeasure": [
        "KWH"
      ]
    }
  ]
}
```

## Misc Notes:
Unsure what this does