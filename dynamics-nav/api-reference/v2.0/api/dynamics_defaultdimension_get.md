---
title: Get defaultDimensions for an entity | Microsoft Docs
description: Gets an item default dimensions in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get entity defaultDimensions
Gets the default dimensions of an entity in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md). 
The following example gets the default dimensions of an entity.

```
GET businesscentralPrefix/companies({id})/defaultDimensions({id})
GET businesscentralPrefix/companies({id})/items({id})/defaultDimensions({id})
GET businesscentralPrefix/companies({id})/customers({id})/defaultDimensions({id})
GET businesscentralPrefix/companies({id})/vendors({id})/defaultDimensions({id})
GET businesscentralPrefix/companies({id})/employees({id})/defaultDimensions({id})
```

## Request header

|Header|Value|
|------|-----|
|Authorization| Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response 

If successful, this method returns a `200 OK` response code and the **default dimensions** in the response body.

## Example 
**Request**

```json
GET https://{businesscentralPrefix}/api/v2.0/companies({companyId})/items({itemId})/defaultDimensions
```

**Response**  
Here is an example of the response.

> [!NOTE]  
> The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
{
    "id": "5b049aad-bde4-ea11-bbf2-00155df3a615",
    "parentId": "53049aad-bde4-ea11-bbf2-00155df3a615",
    "dimensionId": "47c99ea7-bde4-ea11-bbf2-00155df3a615",
    "dimensionCode": "DEPARTMENT",
    "dimensionValueId": "49c99ea7-bde4-ea11-bbf2-00155df3a615",
    "dimensionValueCode": "SALES",
    "postingValidation": " "
} 
```

## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)    
[defaultdimension](../resources/dynamics_defaultdimension.md)    
[Delete defaultdimension](../api/dynamics_defaultdimension_Delete.md)    
[Create defaultdimension](../api/dynamics_defaultdimension_Create.md)    
[Update defaultdimension](../api/dynamics_defaultdimension_Update.md)    
