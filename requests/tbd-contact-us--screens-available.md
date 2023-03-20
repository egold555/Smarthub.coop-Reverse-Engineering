# NAME Request
Short description of the request
```
Method: POST
URL: /services/secured/mobile/contact-us/screens-available
Requires Auth: Yes
```
## Additional Headers:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  content-type   | application/json;    |




## Post Body:
```json
[
  {
    "cabId": {
      "acctNbr": REDACTED,
      "companyId": "REDACTED",
      "custNbr": REDACTED,
      "enterpriseId": "REDACTED",
      "links": {},
      "provider": "ELM",
      "systemID": {
        "companyId": "REDACTED",
        "customerId": "",
        "enterpriseId": "REDACTED",
        "id": 0,
        "systemOfRecord": "UTILITY"
      },
      "systemOfRecord": "UTILITY"
    },
    "cabSummaryAgreementStatus": 1,
    "cabSummaryService": "ELEC",
    "cabSummaryTotalAmountDue": 0
  }
]
```

## Response:
```json
{
  "showReportOutage": false,
  "showReportCommunicationsIssue": false,
  "showGeneralInquiry": true,
  "showOutageTable": false,
  "showCommunicationsIssuesTable": false,
  "showServiceRequestsTable": false,
  "showLocations": true
}
```

## Misc Notes:
Unsure what this method does yet