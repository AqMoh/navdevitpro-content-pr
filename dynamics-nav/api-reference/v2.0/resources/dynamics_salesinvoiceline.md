---
title: salesInvoiceLine resource type | Microsoft Docs
description: A sales invoice line object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/22/2020
ms.author: solsen
---

# salesInvoiceLine resource type
Represents a sales invoice line in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET salesInvoiceLine](../api/dynamics_salesInvoiceLine_Get.md)|salesInvoiceLine|Gets a sales invoice line object.|
|[DELETE salesInvoiceLine](../api/dynamics_salesInvoiceLine_Delete.md)|none|Deletes a sales invoice line object.|
|[POST salesInvoiceLine](../api/dynamics_salesInvoiceLine_Create.md)|salesInvoiceLine|Creates a sales invoice line object.|
|[PATCH salesInvoiceLine](../api/dynamics_salesInvoiceLine_Update.md)|salesInvoiceLine|Updates a sales invoice line object.|




## Navigation

| Navigation |Return Type| Description |    
|:----------|:----------|:-----------------|
|[salesInvoice](../resources/dynamics_salesinvoice.md)|salesInvoice |Gets the salesinvoice of the salesInvoiceLine.|
|[item](../resources/dynamics_item.md)|item |Gets the item of the salesInvoiceLine.|
|[account](../resources/dynamics_account.md)|account |Gets the account of the salesInvoiceLine.|
|[unitOfMeasure](../resources/dynamics_unitofmeasure.md)|unitOfMeasure |Gets the unitofmeasure of the salesInvoiceLine.|
|[itemVariant](../resources/dynamics_itemvariant.md)|itemVariant |Gets the itemvariant of the salesInvoiceLine.|
|[dimensionSetLines](../resources/dynamics_dimensionsetlines.md)|dimensionSetLines |Gets the dimensionsetlines of the salesInvoiceLine.|


## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|documentId|GUID|The ID of the parent sales invoice line. |
|sequence|integer|The line sequence number.|
|itemId|GUID|The ID of the item in the sales invoice line.|
|accountId|GUID|The id of the account that the sales invoice line is related to. |
|lineType|[NAV.invoiceLineAggLineType](../resources/dynamics_complextypes.md)|The type of thesales invoice line. It can be "Comment", "Account", "Item", "Resource" Value", "Fixed Asset" or "Charge".|
|lineObjectNumber|string|The number of the object (account or item) of the sales invoice line.|
|description|string|Specifies the description of the sales invoice line.|
|unitOfMeasureId|GUID|The ID of unit of measure for the sales invoice line.|
|unitOfMeasureCode|string|The code of unit of measure for the sales invoice line.|
|unitPrice|decimal|Specifies the price for one unit of the item in the specified sales invoice line.|
|quantity|decimal|The quantity of the item in the sales invoice line.|
|discountAmount|decimal|The sales invoice line discount amount.|
|discountPercent|decimal|The line discount percent.    |
|discountAppliedBeforeTax|boolean|Specifies whether the discount is applied before tax.|
|amountExcludingTax|decimal|The line amount excluding the tax. Read-Only.|
|taxCode|string|The tax code for the line.       |
|taxPercent|decimal|The tax percent for the line. Read-Only.|
|totalTaxAmount|decimal|The total tax amount for the sales invoice line. Read-Only.|
|amountIncludingTax|decimal|The total amount for the line including tax. Read-Only.|
|invoiceDiscountAllocation|decimal|The sales invoice line discount allocation is the sales invoice line discount distributed on the total amount. Read-Only.|
|netAmount|decimal|The net amount is the amount including all discounts (taken from the sales invoice line). Read-Only.|
|netTaxAmount|decimal|The net tax amount is the tax amount calculated from net amount. Read-Only.|
|netAmountIncludingTax|decimal|The net amount including tax is the total net amount including tax. Read-Only.|
|shipmentDate|date|The date the item in the line is expected to ship.|
|itemVariantId|GUID|The ID of the item variant in the sales invoice line.|


## JSON representation

Here is a JSON representation of the salesInvoiceLine resource.


```json
{
   "id": "GUID",
   "documentId": "GUID",
   "sequence": "integer",
   "itemId": "GUID",
   "accountId": "GUID",
   "lineType": "NAV.invoiceLineAggLineType",
   "lineObjectNumber": "string",
   "description": "string",
   "unitOfMeasureId": "GUID",
   "unitOfMeasureCode": "string",
   "unitPrice": "decimal",
   "quantity": "decimal",
   "discountAmount": "decimal",
   "discountPercent": "decimal",
   "discountAppliedBeforeTax": "boolean",
   "amountExcludingTax": "decimal",
   "taxCode": "string",
   "taxPercent": "decimal",
   "totalTaxAmount": "decimal",
   "amountIncludingTax": "decimal",
   "invoiceDiscountAllocation": "decimal",
   "netAmount": "decimal",
   "netTaxAmount": "decimal",
   "netAmountIncludingTax": "decimal",
   "shipmentDate": "date",
   "itemVariantId": "GUID"
}
```
## See also

[GET salesInvoiceLine](../api/dynamics_salesInvoiceLine_Get.md)
[DELETE salesInvoiceLine](../api/dynamics_salesInvoiceLine_Delete.md)
[POST salesInvoiceLine](../api/dynamics_salesInvoiceLine_Create.md)
[PATCH salesInvoiceLine](../api/dynamics_salesInvoiceLine_Update.md)

