---
title: GET attachments | Microsoft Docs
description: Gets a attachments object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get attachments
Retrieve the properties and relationships of an attachments object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).
```
GET businesscentralPrefix/companies({id})/attachments$filter=parentId eq {journalLineId}
```

> [!NOTE]  
> Please note the $filter applied to attachment API. The filter is applied to get attachments for a specific entity. 


## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and an **attachments** object in the response body.

## Example

**Request**

Here is an example of the request.
```json
GET https://{businesscentralPrefix}/api/v1.0/companies({id})/attachments$filter=parentId eq {journalLineId}
```

**Response**

Here is an example of the response. 

> [!NOTE]  
>   The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
{   
    "id": "b282a6f1-bfe3-ea11-aa60-000d3ad7cacb",
    "parentId": "0a077d18-45e3-ea11-bb43-000d3a2feca1",
    "fileName": "myPDF.pdf",
    "byteSize": 0,
    "lastModifiedDateTime": "2020-08-21T15:06:53Z",
    "parentType": "Journal"   
}
```

## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)    
[attachment](../resources/dynamics_attachment.md)    
[Delete attachment](dynamics_attachment_Delete.md)    
[Create attachment](dynamics_attachment_Create.md)    
[Update attachment](dynamics_attachment_Update.md)    
