---
title: CREATE itemCategories | Microsoft Docs
description: Creates a itemCategory object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Create itemCategories
Create an item category object [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).
```
POST businesscentralPrefix/companies({id})/itemCategories
```

## Request headers

|Header       |Value                    |
|-------------|-------------------------|
|Authorization|Bearer {token}. Required.|
|Content-Type |application/json         |

## Request body
In the request body, supply a JSON representation of an **itemCategories** object.

## Response
If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.

## Example

**Request**

Here is an example of a request.

```json
POST https://{businesscentralPrefix}/api/v2.0/companies({id})/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

**Response**

Here is an example of the response. 

> [!NOTE]  
>   The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "dd1a6a90-44e3-ea11-bb43-000d3a2feca1",
    "code": "CHAIR",
    "displayName": "Office Chair",
    "lastModifiedDateTime": "2020-08-21T00:24:31.777Z"
}
```

## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)     
[itemCategory](../resources/dynamics_itemCategory.md)  
<!--links-->

