---
title: itemCategory resource type | Microsoft Docs
description: An item category object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 01/29/2021
ms.author: solsen
---

<!-- START>DO_NOT_EDIT -->
<!-- IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT. -->
# itemCategory resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

Represents an item category in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods

| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET itemCategory](../api/dynamics_itemCategory_Get.md)|itemCategory|Gets a item category object.|
|[DELETE itemCategory](../api/dynamics_itemCategory_Delete.md)|none|Deletes a item category object.|
|[POST itemCategory](../api/dynamics_itemCategory_Create.md)|itemCategory|Creates a item category object.|
|[PATCH itemCategory](../api/dynamics_itemCategory_Update.md)|itemCategory|Updates a item category object.|



## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|code|string|The code of the item category.|
|displayName|string|Specifies the item category's name. This name will appear on all sales documents for the item category.|
|lastModifiedDateTime|datetime|The last datetime the item category was modified. Read-Only.|

## JSON representation

Here is a JSON representation of the itemCategory resource.


```json
{
    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```
<!-- IMPORTANT: END>DO_NOT_EDIT -->


## See Also
[GET itemCategory](../api/dynamics_itemCategory_Get.md)
[DELETE itemCategory](../api/dynamics_itemCategory_Delete.md)
[POST itemCategory](../api/dynamics_itemCategory_Create.md)
[PATCH itemCategory](../api/dynamics_itemCategory_Update.md)
