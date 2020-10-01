---
title: GET shipmentMethods | Microsoft Docs
description: Gets a shipmentMethod object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get shipmentMethods
Retrieve the properties and relationships of a shipment method object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v1.0/endpoints-apis-for-dynamics.md).

```
GET businesscentralPrefix/companies({id})/shipmentMethods({id})
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and a **shipmentMethods** object in the response body.

## Example

**Request**

Here is an example of the request.
```json
GET https://{businesscentralPrefix}/api/v1.0/companies({id})/shipmentMethods({id})
```

**Response**

Here is an example of the response. 

> [!NOTE]  
>   The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
{
    "id": "87a5738a-44e3-ea11-bb43-000d3a2feca1",
    "code": "CFR",
    "displayName": "Cost and Freight",
    "lastModifiedDateTime": "2020-08-21T00:24:14.287Z"
}
```



## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)    
[shipmentmethod](../resources/dynamics_shipmentmethod.md)    
[Delete shipmentmethod](../api/dynamics_shipmentmethod_Delete.md)    
[Create shipmentmethod](../api/dynamics_shipmentmethod_Create.md)    
[Update shipmentmethod](../api/dynamics_shipmentmethod_Update.md)    
