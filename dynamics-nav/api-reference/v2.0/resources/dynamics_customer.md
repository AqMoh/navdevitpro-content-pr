---
title: customer resource type | Microsoft Docs
description: A customer object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/24/2020
ms.author: solsen
---

# customer resource type
Represents a customer in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET customer](../api/dynamics_customer_Get.md)|customer|Gets a customer object.|
|[DELETE customer](../api/dynamics_customer_Delete.md)|none|Deletes a customer object.|
|[POST customer](../api/dynamics_customer_Create.md)|customer|Creates a customer object.|
|[PATCH customer](../api/dynamics_customer_Update.md)|customer|Updates a customer object.|




## Navigation

| Navigation |Return Type| Description |    
|:----------|:----------|:-----------------|
|[countryRegion](../resources/dynamics_countryregion.md)|countryRegion |Gets the countryregion of the customer.|
|[currency](../resources/dynamics_currency.md)|currency |Gets the currency of the customer.|
|[paymentTerm](../resources/dynamics_paymentterm.md)|paymentTerm |Gets the paymentterm of the customer.|
|[shipmentMethod](../resources/dynamics_shipmentmethod.md)|shipmentMethod |Gets the shipmentmethod of the customer.|
|[paymentMethod](../resources/dynamics_paymentmethod.md)|paymentMethod |Gets the paymentmethod of the customer.|
|[customerFinancialDetail](../resources/dynamics_customerfinancialdetail.md)|customerFinancialDetail |Gets the customerfinancialdetail of the customer.|
|[picture](../resources/dynamics_picture.md)|picture |Gets the picture of the customer.|
|[defaultDimensions](../resources/dynamics_defaultdimensions.md)|defaultDimensions |Gets the defaultdimensions of the customer.|
|[agedAccountsReceivable](../resources/dynamics_agedaccountsreceivable.md)|agedAccountsReceivable |Gets the agedaccountsreceivable of the customer.|


## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|number|string|Specifies the number of the customer.|
|displayName|string|Specifies the customer's name. This name will appear on all sales documents for the customer.|
|type|NAV.contactType|Specifies the type of customer, can be "Company" or "Person".|
|addressLine1|string|Specifies the customer's address. This address will appear on all sales documents for the customer.|
|addressLine2|string|Specifies the customer's address. This address will appear on all sales documents for the customer.|
|city|string|Specifies the customer's city.|
|state|string|Specifies the customer's state.|
|country|string|Specifies the customer's country.|
|postalCode|string|Specifies the customer's postal code.|
|phoneNumber|string|Specifies the customer's telephone number.|
|email|string|Specifies the customer's email address.|
|website|string|Specifies the customer's home page address.|
|taxLiable|boolean|Specifies if the customer or vendor is liable for sales tax. Set to **true** if the customer is tax liable.|
|taxAreaId|GUID|Specifies which tax area the customer belongs to.|
|taxAreaDisplayName|string|Specified the display name of the tax area the customer belongs to.|
|taxRegistrationNumber|string|Specified the tax registration number of the customer.|
|currencyId|GUID|Specifies which currency the customer uses.|
|currencyCode|string|The default currency code for the customer.|
|paymentTermsId|GUID|Specifies which payment term the customer uses.|
|shipmentMethodId|GUID|Specifies which shipment method the customer uses.|
|paymentMethodId|GUID|Specifies which payment method the customer uses.|
|blocked|NAV.customerBlocked|Specifies which transactions with the customer cannot be posted. It can be " ", "Ship", "Invoice" or "All".|
|lastModifiedDateTime|datetime|The last datetime the customer was modified. Read-Only.|


## JSON representation

Here is a JSON representation of the customer resource.


```json
{
   "id": "GUID",
   "number": "string",
   "displayName": "string",
   "type": "NAV.contactType",
   "addressLine1": "string",
   "addressLine2": "string",
   "city": "string",
   "state": "string",
   "country": "string",
   "postalCode": "string",
   "phoneNumber": "string",
   "email": "string",
   "website": "string",
   "taxLiable": "boolean",
   "taxAreaId": "GUID",
   "taxAreaDisplayName": "string",
   "taxRegistrationNumber": "string",
   "currencyId": "GUID",
   "currencyCode": "string",
   "paymentTermsId": "GUID",
   "shipmentMethodId": "GUID",
   "paymentMethodId": "GUID",
   "blocked": "NAV.customerBlocked",
   "lastModifiedDateTime": "datetime"
}
```
## See also

[GET customer](../api/dynamics_customer_Get.md)
[DELETE customer](../api/dynamics_customer_Delete.md)
[POST customer](../api/dynamics_customer_Create.md)
[PATCH customer](../api/dynamics_customer_Update.md)

