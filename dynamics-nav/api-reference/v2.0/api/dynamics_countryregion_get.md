---
title: GET countryRegions | Microsoft Docs
description: Gets a countryRegion object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get countriesRegions
Retrieve the properties and relationships of a countries regions object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).
```
GET businesscentralPrefix/companies({id})/countriesRegions({id})
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and a **countriesRegions** object in the response body.

## Example

**Request**

Here is an example of the request.
```json
GET https://{businesscentralPrefix}/api/v2.0/companies({id})/countriesRegions({id})
```

**Response**

Here is an example of the response. 

> [!NOTE]  
>   The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
{
    "id": "44a5738a-44e3-ea11-bb43-000d3a2feca1",
    "code": "AE",
    "displayName": "United Arab Emirates",
    "addressFormat": "City+ZIP Code",
    "lastModifiedDateTime": "2020-08-21T00:24:13.54Z"
}
```

## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)
[countryregion](../resources/dynamics_countryregion.md)[Delete countryregion](../api/dynamics_countryregion_Delete.md)
[Create countryregion](../api/dynamics_countryregion_Create.md)
[Update countryregion](../api/dynamics_countryregion_Update.md)
