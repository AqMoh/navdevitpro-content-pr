---
title: picture resource type | Microsoft Docs
description: A picture object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/22/2020
ms.author: solsen
---

# picture resource type
Represents a picture in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET picture](../api/dynamics_picture_Get.md)|picture|Gets a picture object.|
|[DELETE picture](../api/dynamics_picture_Delete.md)|none|Deletes a picture object.|
|[PATCH picture](../api/dynamics_picture_Update.md)|picture|Updates a picture object.|






## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|parentType|[NAV.pictureEntityParentType](../resources/dynamics_complextypes.md)|The type of the parent document of the picture. It can be "Customer","Item", "Vendor", "Employee". |
|width|integer|The width of the picture.|
|height|integer|The height of the picture.|
|contentType|string|The media type of the picture.|
|pictureContent|stream|The picture's content.|


## JSON representation

Here is a JSON representation of the picture resource.


```json
{
   "id": "GUID",
   "parentType": "NAV.pictureEntityParentType",
   "width": "integer",
   "height": "integer",
   "contentType": "string",
   "pictureContent": "stream"
}
```
## See also

[GET picture](../api/dynamics_picture_Get.md)
[DELETE picture](../api/dynamics_picture_Delete.md)
[PATCH picture](../api/dynamics_picture_Update.md)

