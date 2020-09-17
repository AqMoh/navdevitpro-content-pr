---
title: CREATE paymentMethods | Microsoft Docs
description: Creates a paymentMethod object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/15/2020
ms.author: solsen
---

# Create paymentMethods
Create a payment method object in D[!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).
```
POST businesscentralPrefix/companies({id})/paymentMethods
```

## Request headers

|Header         |Value                        |
|---------------|-----------------------------|
|Authorization  |Bearer {token}. Required.    |
|Content-Type   |application/json             |

## Request body
In the request body, supply a JSON representation of a **paymentMethods** object.

## Response
If successful, this method returns ```201 Created``` response code and a **paymentMethods** object in the response body.

## Example

**Request**

Here is an example of a request.

```json
POST https://{businesscentralPrefix}/api/v2.0/companies({id})/paymentMethods
Content-type: application/json

{
    "id": "3a196a90-44e3-ea11-bb43-000d3a2feca1",
    "code": "ACCOUNT",
    "displayName": "Payment on account",
    "lastModifiedDateTime": "2020-08-21T00:48:51.487Z"
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
    "id": "3a196a90-44e3-ea11-bb43-000d3a2feca1",
    "code": "ACCOUNT",
    "displayName": "Payment on account",
    "lastModifiedDateTime": "2020-08-21T00:48:51.487Z"
}
```

## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)     
[paymentMethod](../resources/dynamics_paymentMethod.md)  
<!--links-->

