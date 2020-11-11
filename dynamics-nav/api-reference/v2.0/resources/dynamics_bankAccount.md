---
title: bankAccount resource type | Microsoft Docs
description: A bank account object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# bankAccount resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

Represents a bank account in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET bankAccount](../api/dynamics_bankAccount_Get.md)|bankAccount|Gets a bank account object.|
|[DELETE bankAccount](../api/dynamics_bankAccount_Delete.md)|none|Deletes a bank account object.|
|[POST bankAccount](../api/dynamics_bankAccount_Create.md)|bankAccount|Creates a bank account object.|
|[PATCH bankAccount](../api/dynamics_bankAccount_Update.md)|bankAccount|Updates a bank account object.|






## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|number|string|Specifies the number of the bank account.|
|displayName|string|Specifies the bank account's name. This name will appear on all sales documents for the bank account.|


## JSON representation

Here is a JSON representation of the bankAccount resource.


```json
{
   "id": "GUID",
   "number": "string",
   "displayName": "string"
}
```
## See also

[GET bankAccount](../api/dynamics_bankAccount_Get.md)   
[DELETE bankAccount](../api/dynamics_bankAccount_Delete.md)   
[POST bankAccount](../api/dynamics_bankAccount_Create.md)   
[PATCH bankAccount](../api/dynamics_bankAccount_Update.md)   

