---
title: companyInformation resource type | Microsoft Docs
description: A company information object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 11/11/2020
ms.author: solsen
---

# companyInformation resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

Represents a company information in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET companyInformation](../api/dynamics_companyInformation_Get.md)|companyInformation|Gets a company information object.|
|[PATCH companyInformation](../api/dynamics_companyInformation_Update.md)|companyInformation|Updates a company information object.|




## Navigation

| Navigation |Return Type| Description |    
|:----------|:----------|:-----------------|
|[countryRegion](dynamics_countryregion.md)|countryRegion |Gets the countryregion of the companyInformation.|


## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|displayName|string|Specifies the company information's name. This name will appear on all sales documents for the company information.|
|addressLine1|string|Specifies the company information's address. This address will appear on all sales documents for the company information.|
|addressLine2|string|Specifies the company information's address. This address will appear on all sales documents for the company information.|
|city|string|Specifies the company information's city.|
|state|string|Specifies the company information's state.|
|country|string|Specifies the company information's country.|
|postalCode|string|Specifies the company information's postal code.|
|phoneNumber|string|Specifies the company information's telephone number.|
|faxNumber|string|The company's fax number.   |
|email|string|Specifies the company information's email address.|
|website|string|Specifies the company information's home page address.|
|taxRegistrationNumber|string|Specified the tax registration number of the company information.|
|currencyCode|string|The default currency code for the company information.|
|currentFiscalYearStartDate|date|The company's current fiscal year start date. Read-Only.|
|industry|string|The industry the company is part of.|
|picture|stream|The company information's picture.|
|lastModifiedDateTime|datetime|The last datetime the company information was modified. Read-Only.|


## JSON representation

Here is a JSON representation of the companyInformation resource.


```json
{
   "id": "GUID",
   "displayName": "string",
   "addressLine1": "string",
   "addressLine2": "string",
   "city": "string",
   "state": "string",
   "country": "string",
   "postalCode": "string",
   "phoneNumber": "string",
   "faxNumber": "string",
   "email": "string",
   "website": "string",
   "taxRegistrationNumber": "string",
   "currencyCode": "string",
   "currentFiscalYearStartDate": "date",
   "industry": "string",
   "picture": "stream",
   "lastModifiedDateTime": "datetime"
}
```
## See also

[GET companyInformation](../api/dynamics_companyInformation_Get.md)   
[PATCH companyInformation](../api/dynamics_companyInformation_Update.md)   

