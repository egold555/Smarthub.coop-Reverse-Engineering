# Payment Request
Returns information about how the current user is paying for their electricity.
```
Method: GET
URL: https://elmhurstmutual.smarthub.coop/services/secured/gatewayPayments/stored/COMPANY_ID?customerId=REDACTED&paymentAppCd=REC
Requires Auth: Yes
```
## Request Parameters:
| Key             | Value                              |
| --------------- | -----------------------------------|
|  COMPANY_ID     |   Company ID found in [Company Settings](company-settings.md)  |
| customerId      |   Customer id is `custNbr` + `_` + `acctNbt` from [Customer Account Billing](customer-account-billing.md)  |
| paymentAppCd    |   REC -- No clue what else goes here, but it seems to always be `REC` |

## Response:
```json
[
	{
		"companyID": "REDACTED",
		"accountNbr": "REDACTED",
		"typeServiceGrp": "ELEC",
		"customerNbr": "REDACTED",
		"cardSw": true,
		"paymentAppCd": "REC",
		"startDate": 1675231200000,
		"account": {
			"cardAcctType": "Credit",
			"creditCardType": "REDACTED",
			"creditCardCode": "REDACTED",
			"maskedNbr": "*************REDACTED",
			"expireMthYr": "REDACTED",
			"firstName": "REDACTED",
			"lastName": "REDACTED",
			"addr1": "REDACTED",
			"city": "REDACTED",
			"state": "REDACTED",
			"zip": "REDACTED",
			"description": "REDACTED"
		},
		"gatewayRecordId": "REDACTED"
	}
]

```