# User Permissions Request
Returns some sort of list of permissions for the user? Still unsure how this is used
```
Method: GET
URL: https://elmhurstmutual.smarthub.coop/services/secured/authorization/permissions?userId=email%40gmail.com&domain=elmhurstmutual
Requires Auth: Yes
```
## Request Parameters:
| Key             | Value                              |
| --------------- | -----------------------------------|
| userId  | Email of your account    |
| domain  | elmhurstmutual  -- Needs to be the same as the subdomain  |


## Response:
```json
[
	{ "name": "troubleTicketAccess", "realm": "elmhurstmutual" },
	{ "name": "providerAccess", "realm": "elmhurstmutual" },
	{ "name": "MODIFY_ROUND_UPS", "realm": "elmhurstmutual" },
	{ "name": "serviceOrderAccess", "realm": "elmhurstmutual" },
	{ "name": "ViewCustomerData", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_PROVIDER_BILLING", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_SERVICE_BILLING", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_TROUBLE_TICKET_ADMIN", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_BUDGET_BILLING_ENROLLMENT", "realm": "elmhurstmutual" },
	{ "name": "createTroubleTicket", "realm": "elmhurstmutual" },
	{ "name": "payNow", "realm": "elmhurstmutual" },
	{ "name": "makePayments", "realm": "elmhurstmutual" },
	{ "name": "queryGatewayPaymentStatus", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_WORKFLOW_TASKS", "realm": "elmhurstmutual" },
	{ "name": "smartHub", "realm": "elmhurstmutual" },
	{ "name": "accountLookup", "realm": "elmhurstmutual" },
	{ "name": "serviceLocationAccess", "realm": "elmhurstmutual" },
	{ "name": "MODIFY_CONTACT", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_CHARGES", "realm": "elmhurstmutual" },
	{ "name": "currentOutageAccess", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_MISCELLANEOUS_RECEIVABLES", "realm": "elmhurstmutual" },
	{ "name": "initiateReconnect", "realm": "elmhurstmutual" },
	{ "name": "manageGatewayCustomerSecurityInfo", "realm": "elmhurstmutual" },
	{ "name": "customerContact", "realm": "elmhurstmutual" },
	{ "name": "performCreditCheck", "realm": "elmhurstmutual" },
	{ "name": "outageReportAccess", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_CONTACT_EVENTS", "realm": "elmhurstmutual" },
	{ "name": "MODIFY_INVOICE_SETTINGS", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_CREDIT_RATING", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_READINGS", "realm": "elmhurstmutual" },
	{ "name": "customerInformationAccess", "realm": "elmhurstmutual" },
	{ "name": "usageAccess", "realm": "elmhurstmutual" },
	{ "name": "updateServiceOrder", "realm": "elmhurstmutual" },
	{ "name": "createServiceOrder", "realm": "elmhurstmutual" },
	{ "name": "MODIFY_ORDER_REQUEST_PAYMENTS", "realm": "elmhurstmutual" },
	{ "name": "customerContactsAccess", "realm": "elmhurstmutual" },
	{ "name": "registerAnnualMeeting", "realm": "elmhurstmutual" },
	{ "name": "paymentHistoryAccess", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_MISCELLANEOUS_RECEIVABLE_INVOICES", "realm": "elmhurstmutual" },
	{ "name": "queryGatewayBankInformation", "realm": "elmhurstmutual" },
	{ "name": "CREATE_BUDGET_BILLING_ENROLLMENT", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_ORDER_REQUEST_PAYMENTS", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_ROUND_UPS", "realm": "elmhurstmutual" },
	{ "name": "CREATE_ROUND_UPS", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_SERVICE_ORDER", "realm": "elmhurstmutual" },
	{ "name": "billingAccess", "realm": "elmhurstmutual" },
	{ "name": "consumerReadMeterAccess", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_WORKFLOW_TEMPLATES", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_CONTACT", "realm": "elmhurstmutual" },
	{ "name": "manageGatewayStoredPayments", "realm": "elmhurstmutual" },
	{ "name": "smartHubMyServices", "realm": "elmhurstmutual" },
	{ "name": "meterInformationAccess", "realm": "elmhurstmutual" },
	{ "name": "MODIFY_BUDGET_BILLING_ENROLLMENT", "realm": "elmhurstmutual" },
	{ "name": "MODIFY_CHARGES", "realm": "elmhurstmutual" },
	{ "name": "ratesAccess", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_TROUBLE_TICKET", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_INVOICE_SETTINGS", "realm": "elmhurstmutual" },
	{ "name": "editCustomerInformation", "realm": "elmhurstmutual" },
	{ "name": "reportOutages", "realm": "elmhurstmutual" },
	{ "name": "ACCESS_LOCATION_SETUP", "realm": "elmhurstmutual" }
]

```

## Misc Notes:
Unsure what this request is actually used for