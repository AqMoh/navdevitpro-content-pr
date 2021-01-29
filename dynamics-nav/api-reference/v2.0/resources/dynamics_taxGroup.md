---
title: taxGroup resource type | Microsoft Docs
description: A tax group object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: reference
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 01/29/2021
ms.author: solsen
---

<!-- START>DO_NOT_EDIT -->
<!-- IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT. -->
# taxGroup resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

Represents a tax group in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods

| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET taxGroup](../api/dynamics_taxgroup_get.md)|taxGroup|Gets a tax group object.|
|[DELETE taxGroup](../api/dynamics_taxgroup_delete.md)|none|Deletes a tax group object.|
|[POST taxGroup](../api/dynamics_taxgroup_create.md)|taxGroup|Creates a tax group object.|
|[PATCH taxGroup](../api/dynamics_taxgroup_update.md)|taxGroup|Updates a tax group object.|



## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|code|string|The code of the tax group.|
|displayName|string|Specifies the tax group's name. This name will appear on all sales documents for the tax group.|
|taxType|NAV.taxBufferType|Specifies the type of tax. It can be "Sales Tax" or "VAT".|
|lastModifiedDateTime|datetime|The last datetime the tax group was modified. Read-Only.|

## JSON representation

Here is a JSON representation of the taxGroup resource.


```json
{
    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "taxType": "NAV.taxBufferType",
    "lastModifiedDateTime": "datetime"
}
```
<!-- IMPORTANT: END>DO_NOT_EDIT -->



## See Also
[GET taxGroup](../api/dynamics_taxGroup_Get.md)
[DELETE taxGroup](../api/dynamics_taxGroup_Delete.md)
[POST taxGroup](../api/dynamics_taxGroup_Create.md)
[PATCH taxGroup](../api/dynamics_taxGroup_Update.md)
