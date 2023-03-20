# Meter Graph Request (TBA)
NEED TO FINISH THIS
```
Method: GET
URL: /services/secured/readings/graph/SERVICE_LOCATION/ACCOUNT_NUMBER?startDateTime=1641024000000&endDateTime=1678262400000&applicationName=CONSUMER&graphUnitOfMeasure=KWH&timeFrame=MONTHLY
Requires Auth: Yes
```

## Request Parameters:
## Request Parameters:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  ACCOUNT_NUMBER |  Found in the [user login](01-login.md)   |
|  SERVICE_LOCATION |  Found in the [user login](01-login.md)   |


## Response:
```json
[
  {
    "meterLocation": "--REDACTED--",
    "readings": [
      {
        "meterId": "--REDACTED--",
        "parentMeterId": "",
        "channel": 1,
        "flowDirection": "FORWARD",
        "profile": {
          "substituteCumulativeInterpolatedForMissingIntervals": false,
          "useRawIntervalIfVeeIntervalMissing": true,
          "hasCumulative": true,
          "monthly": "CUMULATIVE",
          "daily": "CUMULATIVE",
          "hourly": "SHOW_IF_INTERVALS_EXISTS",
          "fiveMinute": "NEVER_SHOW",
          "actual": "NEVER_SHOW"
        },
        "reads": [
          {
            "interval": {
              "start": 1674979200000,
              "end": 1675238400000
            },
            "hasIntervals": false,
            "metrics": {
              "average": 198,
              "total": 198,
              "minimum": 198,
              "maximum": 198,
              "totalPrice": 0,
              "numReadings": 1,
              "numMissing": 0
            },
            "revenueMonth": {
              "year": 2023,
              "month": "Feb",
              "monthInt": 2
            }
          },
          {
            "interval": {
              "start": 1675238400000,
              "end": 1678147200000
            },
            "hasIntervals": false,
            "metrics": {
              "total": 1574.94,
              "minimum": 1574.942857142857,
              "maximum": 1574.942857142857,
              "totalPrice": 0,
              "numReadings": 1,
              "numMissing": 0
            },
            "revenueMonth": {
              "year": 9999,
              "month": "Dec",
              "monthInt": 12
            }
          }
        ],
        "metrics": {
          "average": 886.47,
          "total": 1772.94,
          "minimum": 198,
          "maximum": 1574.942857142857,
          "totalPrice": 0,
          "numReadings": 2,
          "numMissing": 0
        },
        "industry": "ELECTRIC",
        "unitOfMeasure": "KWH"
      }
    ]
  }
]
```

## Misc Notes:
timeframe = ACTUAL, HOURLY, DAILY, MONTHLY

ACTUAL and HOURLY don't show anything?
FIVE_HOUR 404's

another endpoint: /services/secured/readings/graph/REDACTED/REDACTED?startDateTime=1676966400000&endDateTime=1678262399999&applicationName=CONSUMER&graphUnitOfMeasure=KWH&timeFrame=DAILY

/services/secured/readings/graph/REDACTED/REDACTED?startDateTime=1678003200000&endDateTime=1678322660167&applicationName=CONSUMER&graphUnitOfMeasure=KWH&timeFrame=DAILY