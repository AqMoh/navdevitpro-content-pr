---
title: incomeStatement resource type | Microsoft Docs
description: An income statement object in Dynamics 365 Business Central.
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
# incomeStatement resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

Represents an income statement in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods

| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET incomeStatement](../api/dynamics_incomeStatement_Get.md)|incomeStatement|Gets a income statement object.|



## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|lineNumber|integer|The income statement item line number.|
|display|string|The income statement item display name.|
|netChange|decimal|The income statement net change. |
|lineType|string|The type of the income statement.|
|indentation|integer|The income statement item indentation used in report layout.|
|dateFilter|date|The date filter used to calculate the income statement items.|

## JSON representation

Here is a JSON representation of the incomeStatement resource.


```json
{
    "id": "GUID",
    "lineNumber": "integer",
    "display": "string",
    "netChange": "decimal",
    "lineType": "string",
    "indentation": "integer",
    "dateFilter": "date"
}
```
<!-- IMPORTANT: END>DO_NOT_EDIT -->


## See Also
[GET incomeStatement](../api/dynamics_incomeStatement_Get.md)
