# NAME Request
Short description of the request
```
Method: POST
URL: /services/weather/summaries?zipCode=98445&start=1678003200000&end=1678322660881
Requires Auth: Yes
```
## Additional Headers:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  content-type   |  application/json;   |




## Post Body:
```json
{
  "columns": [
    {
      "start": "1678003200000",
      "end": "1678089600000"
    },
    {
      "start": "1678089600000",
      "end": "1678176000000"
    },
    {
      "start": "1678176000000",
      "end": "1678262400000"
    },
    {
      "start": "1678262400000",
      "end": "1678322660881"
    }
  ]
}
```

## Response:
```json
[
  {
    "dateTime": 1678176000000,
    "highRead": {
      "dateTime": 1678226400000,
      "temperature": 9.7,
      "windSpeed": 3.3554044,
      "windDirection": 230,
      "dewPoint": 1.3
    },
    "lowRead": {
      "dateTime": 1678251600000,
      "temperature": -1,
      "windSpeed": 4.697566,
      "windDirection": 180,
      "dewPoint": -1
    },
    "avgRead": {
      "dateTime": 1678322660337,
      "temperature": 3.6875,
      "windSpeed": 0,
      "windDirection": 0,
      "dewPoint": 0
    }
  },
  {
    "dateTime": 1678262400000,
    "highRead": {
      "dateTime": 1678312800000,
      "temperature": 7.5,
      "windSpeed": 3.3554044,
      "windDirection": 270,
      "dewPoint": 2
    },
    "lowRead": {
      "dateTime": 1678276800000,
      "temperature": -1.3,
      "windSpeed": 0,
      "windDirection": 2.1,
      "dewPoint": -1.3
    },
    "avgRead": {
      "dateTime": 1678322660337,
      "temperature": 2.16,
      "windSpeed": 0,
      "windDirection": 0,
      "dewPoint": 0
    }
  },
  {
    "dateTime": 1678089600000,
    "highRead": {
      "dateTime": 1678136400000,
      "temperature": 9.4,
      "windSpeed": 9.171439,
      "windDirection": 0,
      "dewPoint": -0.2
    },
    "lowRead": {
      "dateTime": 1678104000000,
      "temperature": -2.6,
      "windSpeed": 0,
      "windDirection": 1.5,
      "dewPoint": -2.7
    },
    "avgRead": {
      "dateTime": 1678322660337,
      "temperature": 3.6760867,
      "windSpeed": 0,
      "windDirection": 0,
      "dewPoint": 0
    }
  },
  {
    "dateTime": 1678003200000,
    "highRead": {
      "dateTime": 1678053600000,
      "temperature": 9.1,
      "windSpeed": 3.3554044,
      "windDirection": 340,
      "dewPoint": -0.5
    },
    "lowRead": {
      "dateTime": 1678017600000,
      "temperature": -4,
      "windSpeed": 0,
      "windDirection": 0,
      "dewPoint": -4.1
    },
    "avgRead": {
      "dateTime": 1678322660337,
      "temperature": 2.3079996,
      "windSpeed": 0,
      "windDirection": 0,
      "dewPoint": 0
    }
  }
]
```

## Misc Notes:
Still unsure exactly what this does, something related to weather and the graph endpoint