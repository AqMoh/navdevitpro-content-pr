---
title: defaultDimensions resource type | Microsoft Docs
description: A default dimensions object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/22/2020
ms.author: solsen
---

# defaultDimensions resource type
Represents a default dimensions in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET defaultDimensions](../api/dynamics_defaultDimensions_Get.md)|defaultDimensions|Gets a default dimensions object.|
|[DELETE defaultDimensions](../api/dynamics_defaultDimensions_Delete.md)|defaultDimensions|Deletes a default dimensions object.|
|[POST defaultDimensions](../api/dynamics_defaultDimensions_Create.md)|defaultDimensions|Creates a default dimensions object.|
|[PATCH defaultDimensions](../api/dynamics_defaultDimensions_Update.md)|defaultDimensions|Updates a default dimensions object.|




## Navigation

| Navigation |Return Type| Description |    
|:----------|:----------|:-----------------|
|[item](../resources/dynamics_item.md)|item |Gets the item of the defaultDimensions.|
|[account](../resources/dynamics_account.md)|account |Gets the account of the defaultDimensions.|
|[dimension](../resources/dynamics_dimension.md)|dimension |Gets the dimension of the defaultDimensions.|
|[dimensionValue](../resources/dynamics_dimensionvalue.md)|dimensionValue |Gets the dimensionvalue of the defaultDimensions.|
|[customer](../resources/dynamics_customer.md)|customer |Gets the customer of the defaultDimensions.|
|[vendor](../resources/dynamics_vendor.md)|vendor |Gets the vendor of the defaultDimensions.|
|[employee](../resources/dynamics_employee.md)|employee |Gets the employee of the defaultDimensions.|


## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|parentId|GUID|The ID of the parent entity. |
|dimensionId|GUID|The unique ID of dimension.|
|dimensionCode|string|The dimension code.|
|dimensionValueId|GUID|The unique ID of the dimension value.|
|dimensionValueCode|string|The dimension value code.  |
|postingValidation|string|Specifies how default dimensions and their values must be used.|


## JSON representation

Here is a JSON representation of the defaultDimensions resource.


```json
{
   "parentId": "GUID",
   "dimensionId": "GUID",
   "dimensionCode": "string",
   "dimensionValueId": "GUID",
   "dimensionValueCode": "string",
   "postingValidation": "string"
}
```
## See also

[GET defaultDimensions](../api/dynamics_defaultDimensions_Get.md)
[DELETE defaultDimensions](../api/dynamics_defaultDimensions_Delete.md)
[POST defaultDimensions](../api/dynamics_defaultDimensions_Create.md)
[PATCH defaultDimensions](../api/dynamics_defaultDimensions_Update.md)

