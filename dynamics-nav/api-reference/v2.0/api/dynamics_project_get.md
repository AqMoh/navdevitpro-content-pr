---
title: GET projects | Microsoft Docs
description: Gets a project object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get projects
Retrieve the properties and relationships of a project object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)]. 


## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).
```
GET businesscentralPrefix/companies({id})/projects({id})
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and an **projects** object in the response body.

## Example

**Request**

Here is an example of the request.
```json
GET https://{businesscentralPrefix}/api/v2.0/companies({id})/projects({id})
```

**Response**

Here is an example of the response. 

```json
{
    "id": "22d7a1c5-bde4-ea11-bbf2-00155df3a615",
    "number": "DEERFIELD, 8 WP",
    "displayName": "Setting up Eight Work Areas"
}
```


## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)    
[project](../resources/dynamics_project.md)    
[Delete project](../api/dynamics_project_Delete.md)    
[Create project](../api/dynamics_project_Create.md)    
[Update project](../api/dynamics_project_Update.md)    
