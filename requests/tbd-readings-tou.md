# NAME Request
Short description of the request
```
Method: POST
URL: /services/secured/readings/tou/SERVICE_LOCATION/ACCOUNT_NUMBER?applicationName=CONSUMER&timeFrame=MONTHLY
Requires Auth: Yes
```

## Request Parameters:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  ACCOUNT_NUMBER |  Found in the [user login](01-login.md)   |
|  SERVICE_LOCATION |  Found in the [user login](01-login.md)   |


## Post Body:
```json
{
  "columns": [
    {
      "start": "1641024000000",
      "end": "1643702400000"
    },
    {
      "start": "1643702400000",
      "end": "1646121600000"
    },
    {
      "start": "1646121600000",
      "end": "1648796400000"
    },
    {
      "start": "1648796400000",
      "end": "1651388400000"
    },
    {
      "start": "1651388400000",
      "end": "1654066800000"
    },
    {
      "start": "1654066800000",
      "end": "1656658800000"
    },
    {
      "start": "1656658800000",
      "end": "1659337200000"
    },
    {
      "start": "1659337200000",
      "end": "1662015600000"
    },
    {
      "start": "1662015600000",
      "end": "1664607600000"
    },
    {
      "start": "1664607600000",
      "end": "1667286000000"
    },
    {
      "start": "1667286000000",
      "end": "1669881600000"
    },
    {
      "start": "1669881600000",
      "end": "1672560000000"
    },
    {
      "start": "1672560000000",
      "end": "1675238400000"
    },
    {
      "start": "1674979200000",
      "end": "1675238400000"
    },
    {
      "start": "1675238400000",
      "end": "1677657600000"
    },
    {
      "start": "1677657600000",
      "end": "1678262400000"
    }
  ]
}
```

## Response:
```json
[]
```

## Misc Notes:
Unsure what this request does yet