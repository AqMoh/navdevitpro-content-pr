---
title: unitOfMeasure resource type | Microsoft Docs
description: An unit of measure object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: reference
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 01/29/2021
ms.author: solsen
---

# unitOfMeasure resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

<!-- START>DO_NOT_EDIT -->
<!-- IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT. -->
Represents an unit of measure in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods

| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET unitOfMeasure](../api/dynamics_unitofmeasure_get.md)|unitOfMeasure|Gets a unit of measure object.|
|[DELETE unitOfMeasure](../api/dynamics_unitofmeasure_delete.md)|none|Deletes a unit of measure object.|
|[POST unitOfMeasure](../api/dynamics_unitofmeasure_create.md)|unitOfMeasure|Creates a unit of measure object.|
|[PATCH unitOfMeasure](../api/dynamics_unitofmeasure_update.md)|unitOfMeasure|Updates a unit of measure object.|



## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|code|string|The code of the unit of measure.|
|displayName|string|Specifies the unit of measure's name. This name will appear on all sales documents for the unit of measure.|
|internationalStandardCode|string|Specifies the unit of measure code expressed according to the UNECE Rec20 standard in connection with electronic sending of sales documents.|
|symbol|string|Specifies a graphical representation of the unit of measure.|
|lastModifiedDateTime|datetime|The last datetime the unit of measure was modified. Read-Only.|

## JSON representation

Here is a JSON representation of the unitOfMeasure resource.


```json
{
    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "internationalStandardCode": "string",
    "symbol": "string",
    "lastModifiedDateTime": "datetime"
}
```
<!-- IMPORTANT: END>DO_NOT_EDIT -->



## See Also
[GET unitOfMeasure](../api/dynamics_unitOfMeasure_Get.md)
[DELETE unitOfMeasure](../api/dynamics_unitOfMeasure_Delete.md)
[POST unitOfMeasure](../api/dynamics_unitOfMeasure_Create.md)
[PATCH unitOfMeasure](../api/dynamics_unitOfMeasure_Update.md)
