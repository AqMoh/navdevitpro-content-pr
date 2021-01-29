---
title: itemVariant resource type | Microsoft Docs
description: An item variant object in Dynamics 365 Business Central.
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
# itemVariant resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

Represents an item variant in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods

| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET itemVariant](../api/dynamics_itemVariant_Get.md)|itemVariant|Gets a item variant object.|
|[DELETE itemVariant](../api/dynamics_itemVariant_Delete.md)|none|Deletes a item variant object.|
|[POST itemVariant](../api/dynamics_itemVariant_Create.md)|itemVariant|Creates a item variant object.|
|[PATCH itemVariant](../api/dynamics_itemVariant_Update.md)|itemVariant|Updates a item variant object.|


## Navigation

| Navigation |Return Type| Description |
|:----------|:----------|:-----------------|
|[item](dynamics_item.md)|item |Gets the item of the itemVariant.|

## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|itemId|GUID|The ID of the item in the item variant.|
|itemNumber|string|The name of the item in the item variant.|
|code|string|The code of the item variant.|
|description|string|Specifies the description of the item variant.|

## JSON representation

Here is a JSON representation of the itemVariant resource.


```json
{
    "id": "GUID",
    "itemId": "GUID",
    "itemNumber": "string",
    "code": "string",
    "description": "string"
}
```
<!-- IMPORTANT: END>DO_NOT_EDIT -->


## See Also
[GET itemVariant](../api/dynamics_itemVariant_Get.md)
[DELETE itemVariant](../api/dynamics_itemVariant_Delete.md)
[POST itemVariant](../api/dynamics_itemVariant_Create.md)
[PATCH itemVariant](../api/dynamics_itemVariant_Update.md)
