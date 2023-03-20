# Customer Billing Request
Gett total amount due for your account, and customer address
```
Method: GET
URL: https://elmhurstmutual.smarthub.coop/services/secured/aggregate/customerAccountBilling/totals?email=email%40gmail.com
Requires Auth: Yes
```
## Request Parameters:
| Key             | Value                                      |
| --------------- | -------------------------------------------|
| email           |  Email address assosated with your account |


## Response:
```json
{
	"totalAmtDue": 0.0,
	"customerAccountBillings": [
		{
			"summary": {
				"id": {
					"custNbr": --REDACTED--,
					"acctNbr": --REDACTED--,
					"provider": "ELM",
					"systemID": { "systemOfRecord": "UTILITY", "enterpriseId": "51249", "companyId": "51249" }
				},
				"isDefaultCustomer": true,
				"accountBalance": 0.0,
				"totalAmtDue": 0.0,
				"totalDueTimestamp": 1676966400000,
				"consClassCd": "",
				"uncollectible": false,
				"agreementStatus": 1,
				"invoiceGroupNumber": 0,
				"invoiceGroupMaster": false,
				"voipAgreementIds": [],
				"primarySrvLocNbr": --REDACTED--,
				"primaryServiceLocation": "--REDACTED--",
				"service": "ELEC",
				"serviceDesc": "ELECTRIC SERVICE",
				"providerDesc": "ELECTRIC SERVICE",
				"dnpSw": "N",
				"bankDraftTimestamp": 1677052800000,
				"reconnectFee": 0.0,
				"reconnectMinDue": 0.0,
				"prepaidAvgDailyAmt": 0.0,
				"accountMessageMap": {},
				"billingInserts": [],
				"billInsertsExist": false,
				"dataUsages": [],
				"persAcctNbr": --REDACTED--,
				"isPrintedBillOn": false,
				"gatewayLocationId": "1",
				"prepaidDisconnectNonPay": false
			},
			"detail": {
				"custName": "ERIC GOLDE",
				"firstName": "ERIC",
				"lastName": "GOLDE",
				"additionalCustomerName": "--REDACTED--",
				"additionalFirstName": "--REDACTED--",
				"additionalLastName": "--REDACTED--",
				"addr1": "--REDACTED--",
				"city": "--REDACTED--",
				"state": "--REDACTED--",
				"zip": "--REDACTED--",
				"email": "--REDACTED--",
				"allowChkPymnt": true,
				"allowCcPymnt": true,
				"currentAmtDue": 0.0,
				"pastAmtDue": 0.0,
				"pastAmtDue2": 0.0,
				"lastBillTimestamp": 1675861667000,
				"currentDueTimestamp": 1676966400000,
				"servLocs": [
					{
						"id": { "srvLocNbr": --REDACTED--, "serviceLocation": "--REDACTED--" },
						"location": "--REDACTED--",
						"address": { "addr1": "--REDACTED--", "city": "--REDACTED--", "state": "--REDACTED--", "zip": "--REDACTED--" },
						"serviceStatus": "ACTIVE",
						"lastBillPrevReadDtTm": 1674979200000,
						"lastBillPresReadDtTm": 1675238400000,
						"meterNumbersToExternalMeterBaseIds": { "--REDACTED--": "--REDACTED--" },
						"activeRateSchedules": [ "1:ELM" ]
					}
				],
				"providers": [ "ELM" ]
			}
		}
	],
	"defaultCustomerIndex": 0
}

```

## Misc Notes:
Email must be the same email as your login email, or elsse the request errors.