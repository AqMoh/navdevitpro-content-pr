---
title: balanceSheet resource type | Microsoft Docs
description: A balance sheet object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# balanceSheet resource type
Represents a balance sheet in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET balanceSheet](../api/dynamics_balanceSheet_Get.md)|balanceSheet|Gets a balance sheet object.|






## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|lineNumber|integer|The balance sheet item line number.|
|display|string|The balance sheet item display name.|
|balance|decimal|Specifies balance sheet's total balance.|
|lineType|string|The type of the balance sheet.|
|indentation|integer|The balance sheet item indentation used in report layout.|
|dateFilter|date|The date filter used to calculate the balance sheet items.|


## JSON representation

Here is a JSON representation of the balanceSheet resource.


```json
{
   "id": "GUID",
   "lineNumber": "integer",
   "display": "string",
   "balance": "decimal",
   "lineType": "string",
   "indentation": "integer",
   "dateFilter": "date"
}
```
## See also

[GET balanceSheet](../api/dynamics_balanceSheet_Get.md)   

