---
title: Get picture | Microsoft Docs
description: A picture object in Dynamics 365 Business Central. 
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get picture
Retrieve the properties and relationships of a picture object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).s
```
GET businesscentralPrefix/companies({companyId})/items({itemId})/picture
GET businesscentralPrefix/companies({companyId})/employee({employeeId})/picture
GET businesscentralPrefix/companies({companyId})/vendor({vendorId})/picture
GET businesscentralPrefix/companies({companyId})/customer({customerId})/picture

```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Response
If successful, this method returns a ```200 OK``` response code and a **picture** object in the response body.

## Example

**Request**

Here is an example of the request. 

**GET Metadata** 

```json
GET https://{businesscentralPrefix}/api/v2.0/companies(companyId)/items(itemId)/picture(itemId)
```
**Response**

Here is an example of the response.

> [!NOTE]  
> The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
{
    "id": "53049aad-bde4-ea11-bbf2-00155df3a615",
    "parentType": "Customer", 
    "width": 400,
    "height": 400,
    "contentType": "image/jpeg",
    "pictureContent@odata.mediaEditLink": "http://onbuyuka-azvm1.europe.corp.microsoft.com:7047/Navision_NAV/api/v2.0/companies(52e03390-bde4-ea11-bbf2-00155df3a615)/customers(53049aad-bde4-ea11-bbf2-00155df3a615)/picture/pictureContent",
    "pictureContent@odata.mediaReadLink": "http://onbuyuka-azvm1.europe.corp.microsoft.com:7047/Navision_NAV/api/v2.0/companies(52e03390-bde4-ea11-bbf2-00155df3a615)/customers(53049aad-bde4-ea11-bbf2-00155df3a615)/picture/pictureContent"
}
```

**GET Content**

```json
GET https://{businesscentralPrefix}/api/v2.0/companies(companyId)/items(itemId)/picture(itemId)/content
```

**Response**

Body is the raw image data. 


## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)    
[picture](../resources/dynamics_picture.md)    
[Delete picture](../api/dynamics_picture_Delete.md)    
[Update picture](../api/dynamics_picture_Update.md)    
