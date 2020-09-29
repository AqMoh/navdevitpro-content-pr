---
title: salesQuote resource type | Microsoft Docs
description: A sales quote object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# salesQuote resource type
Represents a sales quote in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET salesQuote](../api/dynamics_salesQuote_Get.md)|salesQuote|Gets a sales quote object.|
|[DELETE salesQuote](../api/dynamics_salesQuote_Delete.md)|none|Deletes a sales quote object.|
|[POST salesQuote](../api/dynamics_salesQuote_Create.md)|salesQuote|Creates a sales quote object.|
|[PATCH salesQuote](../api/dynamics_salesQuote_Update.md)|salesQuote|Updates a sales quote object.|




## Navigation

| Navigation |Return Type| Description |    
|:----------|:----------|:-----------------|
|[customer](../resources/dynamics_customer.md)|customer |Gets the customer of the salesQuote.|
|[countryRegion](../resources/dynamics_countryregion.md)|countryRegion |Gets the countryregion of the salesQuote.|
|[currency](../resources/dynamics_currency.md)|currency |Gets the currency of the salesQuote.|
|[paymentTerm](../resources/dynamics_paymentterm.md)|paymentTerm |Gets the paymentterm of the salesQuote.|
|[shipmentMethod](../resources/dynamics_shipmentmethod.md)|shipmentMethod |Gets the shipmentmethod of the salesQuote.|
|[salesQuoteLines](../resources/dynamics_salesquotelines.md)|salesQuoteLines |Gets the salesquotelines of the salesQuote.|
|[pdfDocument](../resources/dynamics_pdfdocument.md)|pdfDocument |Gets the pdfdocument of the salesQuote.|
|[attachments](../resources/dynamics_attachments.md)|attachments |Gets the attachments of the salesQuote.|
|[dimensionSetLines](../resources/dynamics_dimensionsetlines.md)|dimensionSetLines |Gets the dimensionsetlines of the salesQuote.|


## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|number|string|Specifies the number of the sales quote.|
|externalDocumentNumber|string|Specifies an external document number for the sales quote.|
|documentDate|date|The quote date.|
|postingDate|date|The date that the sales quote   is posted.|
|dueDate|date|T he date the sales quote is due.|
|customerId|GUID|The unique ID of customer.  |
|customerNumber|string|The customer's number.|
|customerName|string|The customer's name.|
|billToName|string|Bill to name.|
|billToCustomerId|GUID|Bill to customer id.|
|billToCustomerNumber|string|Bill to customer number.|
|shipToName|string|Ship to name.|
|shipToContact|string|Ship to contact.|
|sellToAddressLine1|string|Sell to address line 1.|
|sellToAddressLine2|string|Sell to address line 2.|
|sellToCity|string|Sell to city.|
|sellToCountry|string|Sell to country.|
|sellToState|string|Sell to state.|
|sellToPostCode|string|Sell to post code.|
|billToAddressLine1|string|Bill to address line 1.|
|billToAddressLine2|string|Bill to address line 2.|
|billToCity|string|Bill to city.|
|billToCountry|string|Bill to country.|
|billToState|string|Bill to state.|
|billToPostCode|string|Bill to post code.|
|shipToAddressLine1|string|Ship to address line 1.|
|shipToAddressLine2|string|Ship to address line 2.|
|shipToCity|string|Ship to city.|
|shipToCountry|string|Ship to country.|
|shipToState|string|Ship to state.|
|shipToPostCode|string|Ship to post code.|
|currencyId|GUID|Specifies which currency the sales quote uses.|
|currencyCode|string|The default currency code for the sales quote.|
|paymentTermsId|GUID|Specifies which payment term the sales quote uses.|
|shipmentMethodId|GUID|Specifies which shipment method the sales quote uses.|
|salesperson|string|The salesperson code for the sales quote.|
|discountAmount|decimal|The sales quote discount amount.|
|totalAmountExcludingTax|decimal|The total amount excluding tax. Read-Only.  |
|totalTaxAmount|decimal|The total tax amount for the sales quote. Read-Only.|
|totalAmountIncludingTax|decimal|The total amount including tax. Read-Only.  |
|status|NAV.salesQuoteEntityBufferStatus|Specifies the status of the sales quote. It can be "Draft", "Sent", "Accepted" or "Expired ".|
|sentDate|datetime|The the date and time the quote was sent our to the customer. Read-Only.|
|validUntilDate|date|The date a quote is valid until.|
|acceptedDate|date|The date a sales quote is accepted. Read-Only.|
|lastModifiedDateTime|datetime|The last datetime the sales quote was modified. Read-Only.|
|phoneNumber|string|Specifies the sales quote's telephone number.|
|email|string|Specifies the sales quote's email address.|


## JSON representation

Here is a JSON representation of the salesQuote resource.


```json
{
   "id": "GUID",
   "number": "string",
   "externalDocumentNumber": "string",
   "documentDate": "date",
   "postingDate": "date",
   "dueDate": "date",
   "customerId": "GUID",
   "customerNumber": "string",
   "customerName": "string",
   "billToName": "string",
   "billToCustomerId": "GUID",
   "billToCustomerNumber": "string",
   "shipToName": "string",
   "shipToContact": "string",
   "sellToAddressLine1": "string",
   "sellToAddressLine2": "string",
   "sellToCity": "string",
   "sellToCountry": "string",
   "sellToState": "string",
   "sellToPostCode": "string",
   "billToAddressLine1": "string",
   "billToAddressLine2": "string",
   "billToCity": "string",
   "billToCountry": "string",
   "billToState": "string",
   "billToPostCode": "string",
   "shipToAddressLine1": "string",
   "shipToAddressLine2": "string",
   "shipToCity": "string",
   "shipToCountry": "string",
   "shipToState": "string",
   "shipToPostCode": "string",
   "currencyId": "GUID",
   "currencyCode": "string",
   "paymentTermsId": "GUID",
   "shipmentMethodId": "GUID",
   "salesperson": "string",
   "discountAmount": "decimal",
   "totalAmountExcludingTax": "decimal",
   "totalTaxAmount": "decimal",
   "totalAmountIncludingTax": "decimal",
   "status": "NAV.salesQuoteEntityBufferStatus",
   "sentDate": "datetime",
   "validUntilDate": "date",
   "acceptedDate": "date",
   "lastModifiedDateTime": "datetime",
   "phoneNumber": "string",
   "email": "string"
}
```
## See also

[GET salesQuote](../api/dynamics_salesQuote_Get.md)   
[DELETE salesQuote](../api/dynamics_salesQuote_Delete.md)   
[POST salesQuote](../api/dynamics_salesQuote_Create.md)   
[PATCH salesQuote](../api/dynamics_salesQuote_Update.md)   

