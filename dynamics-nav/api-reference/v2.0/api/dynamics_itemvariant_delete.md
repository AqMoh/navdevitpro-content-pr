---
title: DELETE itemVariants | Microsoft Docs
description: Deletes itemVariant  in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Delete itemVariants
Deletes itemVariants in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).
```
DELETE businesscentralPrefix/companies({id})/itemVariants({id})
DELETE businesscentralPrefix/companies({id})/items({id})/itemVariants({id})
```

## Request headers

|Header         |Value                     |
|---------------|--------------------------|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```204 No Content``` response code and it deletes the itemVariant .

## Example

**Request**

Here is an example of the request.

```json
DELETE https://{businesscentralPrefix}/api/v2.0/companies({id})/itemVariants({id})
```

**Response** 

Here is an example of the response. 

```json
HTTP/1.1 204 No Content
```


## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)    
[itemvariant](../resources/dynamics_itemvariant.md)    
[Get itemvariant](../api/dynamics_itemvariant_Get.md)    
[Create itemvariant](../api/dynamics_itemvariant_Create.md)    
[Update itemvariant](../api/dynamics_itemvariant_Update.md)    
