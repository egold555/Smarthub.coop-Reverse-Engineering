# NAME Request
Some sort of event retriever?
```
Method: GET
URL: /services/secured/courier/event/mobile/email@gmail.com?modifiedAfterDate=1675903442571
Requires Auth: Yes
```


## Request Parameters:
| Key             | Value                              |
| --------------- | -----------------------------------|
|     |     |


## Response:
```json
[
  {
    "domain": "elmhurstmutual",
    "notificationId": "m1+elmhurstmutual+BILL_AVAILABLE+4+785c2e00-a815-11ed-a014-f5da8976a857",
    "notificationType": "BILL_AVAILABLE",
    "subject": "Bill Available",
    "detail": "Your ELECTRIC SERVICE bill is available for the following accounts:\n\nREDACTED\n.",
    "status": "UNREAD",
    "createdDateTime": 1675904568548,
    "modifiedDateTime": 0,
    "metaData": "{\"billList\":[{\"companyName\":\"Elmhurst Mutual Power \\u0026 Light\",\"customerName\":\"REDACTED\",\"customerNbr\":\"REDACTED\",\"accountNbr\":\"REDACTED\",\"serviceList\":[{\"accountNbr\":\"REDACTED\",\"serviceDesc\":\"ELECTRIC SERVICE\",\"serviceAddress\":\"REDACTED\",\"typeService\":\"ELM\"}],\"billDate\":1675861667000,\"paymentDueDate\":1676966400000,\"billAmt\":\"REDACTED\",\"draftDate\":1676966400000,\"draftType\":\"charged\",\"url\":\"https://elmhurstmutual.smarthub.coop\",\"consumerClassCode\":\"N\",\"pastAmt\":\"$0.00\",\"pastAmt30\":\"$0.00\",\"pastAmt60\":\"$0.00\",\"pastAmt90\":\"$0.00\",\"currentAmt\":\"REDACTED\",\"currentRoundUpAmount\":\"$0.00\",\"yearToDateRoundUpAmount\":\"0\",\"invoiceGroupNumber\":\"0\",\"numberOfBills\":\"0\",\"billPrintTypeCode\":\"DOC\",\"serviceStatusCode\":\"1\",\"serviceAddressLine1\":\"REDACTED\",\"cycleControlPenaltyDueDate\":1676966400000,\"cycleControlDelinquent1DueDate\":1679641200000,\"cycleControlCutoffDate\":1680591600000,\"cycleControlConsumptionFromDate\":1672905600000,\"cycleControlConsumptionToDate\":1675324800000,\"cycleControlPrintBillDate\":1675843200000,\"paymentArrangementUDO52\":\"Y\"}]}"
  }
]
```

## Misc Notes:
Not totally sure what this is for.