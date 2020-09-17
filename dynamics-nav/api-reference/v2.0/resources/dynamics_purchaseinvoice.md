---
title: purchaseInvoice resource type | Microsoft Docs
description: A purchase invoice object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/17/2020
ms.author: solsen
---

# purchaseInvoice resource type
Represents an purchase invoice in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET purchaseInvoice](../api/dynamics_purchaseInvoice_Get.md)|purchaseInvoice|Gets a purchase invoice object.|
|[CHANGE purchaseInvoice](../api/dynamics_purchaseInvoice_Change.md)|purchaseInvoice|Changes a purchase invoice object.|
|[DELETE purchaseInvoice](../api/dynamics_purchaseInvoice_Delete.md)|purchaseInvoice|Deletes a purchase invoice object.|
|[POST purchaseInvoice](../api/dynamics_purchaseInvoice_Create.md)|purchaseInvoice|Creates a purchase invoice object.|
|[PATCH purchaseInvoice](../api/dynamics_purchaseInvoice_Update.md)|purchaseInvoice|Updates a purchase invoice object.|


## Bound Actions
post

## Navigation

| Navigation |Return Type| Description |    
|:----------|:----------|:-----------------|
|[vendor](../resources/dynamics_vendor.md)|vendor |Gets the vendor of the purchaseInvoice.|
|[countryRegion](../resources/dynamics_countryregion.md)|countryRegion |Gets the countryregion of the purchaseInvoice.|
|[currency](../resources/dynamics_currency.md)|currency |Gets the currency of the purchaseInvoice.|
|[purchaseInvoiceLines](../resources/dynamics_purchaseinvoicelines.md)|purchaseInvoiceLines |Gets the purchaseinvoicelines of the purchaseInvoice.|
|[pdfDocument](../resources/dynamics_pdfdocument.md)|pdfDocument |Gets the pdfdocument of the purchaseInvoice.|
|[attachments](../resources/dynamics_attachments.md)|attachments |Gets the attachments of the purchaseInvoice.|
|[dimensionSetLines](../resources/dynamics_dimensionsetlines.md)|dimensionSetLines |Gets the dimensionsetlines of the purchaseInvoice.|


## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|number|string|Specifies the number of the purchase invoice.|
|invoiceDate|date|The invoice date .|
|postingDate|date|The date that the purchase invoice   is posted.|
|dueDate|date|T he date the purchase invoice is due.|
|vendorInvoiceNumber|string|The vendor sales order reference for the purchase invoice.|
|vendorId|GUID|The unique ID of vendor.|
|vendorNumber|string|Specifies vendor's number.|
|vendorName|string|Specifies vendor's name.|
|payToName|string|Pay to name of the purchase invoice. |
|payToContact|string|Pay to contact.|
|payToVendorId|GUID|Pay to vendor id.|
|payToVendorNumber|string|Pay to vendor number.|
|shipToName|string|Ship to name.|
|shipToContact|string|Ship to contact.|
|buyFromAddressLine1|string|Buy from address line 1.|
|buyFromAddressLine2|string|Buy from address line 2.|
|buyFromCity|string|Buy from city.|
|buyFromCountry|string|Buy from state.|
|buyFromState|string|Buy from state.|
|buyFromPostCode|string|Buy from country.|
|shipToAddressLine1|string|Ship to address line 1.|
|shipToAddressLine2|string|Ship to address line 2.|
|shipToCity|string|Ship to city.|
|shipToCountry|string|Ship to country.|
|shipToState|string|Ship to state.|
|shipToPostCode|string|Ship to post code.|
|payToAddressLine1|string|Pay to address line 1.|
|payToAddressLine2|string|Pay to address line 2.|
|payToCity|string|Pay to address line 2.|
|payToCountry|string|Pay to country.|
|payToState|string|Pay to state.|
|payToPostCode|string|Pay to post code.|
|currencyId|GUID|Specifies which currency the purchase invoice uses.|
|currencyCode|string|The default currency code for the purchase invoice.|
|pricesIncludeTax|boolean|Specifies whether the prices include Tax or not. Read-Only.|
|discountAmount|decimal|The purchase invoice discount amount.|
|discountAppliedBeforeTax|boolean|Specifies whether the discount is applied before tax.|
|totalAmountExcludingTax|decimal|The total amount excluding tax. Read-Only.  |
|totalTaxAmount|decimal|The total tax amount for the purchase invoice. Read-Only.|
|totalAmountIncludingTax|decimal|The total amount including tax. Read-Only.  |
|status|string|Specifies the status of the purchase invoice.|
|lastModifiedDateTime|datetime|The last datetime the purchase invoice was modified. Read-Only.|


## JSON representation

Here is a JSON representation of the purchaseInvoice resource.


```json
{
   "id": "GUID",
   "number": "string",
   "invoiceDate": "date",
   "postingDate": "date",
   "dueDate": "date",
   "vendorInvoiceNumber": "string",
   "vendorId": "GUID",
   "vendorNumber": "string",
   "vendorName": "string",
   "payToName": "string",
   "payToContact": "string",
   "payToVendorId": "GUID",
   "payToVendorNumber": "string",
   "shipToName": "string",
   "shipToContact": "string",
   "buyFromAddressLine1": "string",
   "buyFromAddressLine2": "string",
   "buyFromCity": "string",
   "buyFromCountry": "string",
   "buyFromState": "string",
   "buyFromPostCode": "string",
   "shipToAddressLine1": "string",
   "shipToAddressLine2": "string",
   "shipToCity": "string",
   "shipToCountry": "string",
   "shipToState": "string",
   "shipToPostCode": "string",
   "payToAddressLine1": "string",
   "payToAddressLine2": "string",
   "payToCity": "string",
   "payToCountry": "string",
   "payToState": "string",
   "payToPostCode": "string",
   "currencyId": "GUID",
   "currencyCode": "string",
   "pricesIncludeTax": "boolean",
   "discountAmount": "decimal",
   "discountAppliedBeforeTax": "boolean",
   "totalAmountExcludingTax": "decimal",
   "totalTaxAmount": "decimal",
   "totalAmountIncludingTax": "decimal",
   "status": "string",
   "lastModifiedDateTime": "datetime"
}
```
## See also

[GET purchaseInvoice](../api/dynamics_purchaseInvoice_Get.md)
[CHANGE purchaseInvoice](../api/dynamics_purchaseInvoice_Change.md)
[DELETE purchaseInvoice](../api/dynamics_purchaseInvoice_Delete.md)
[POST purchaseInvoice](../api/dynamics_purchaseInvoice_Create.md)
[PATCH purchaseInvoice](../api/dynamics_purchaseInvoice_Update.md)

