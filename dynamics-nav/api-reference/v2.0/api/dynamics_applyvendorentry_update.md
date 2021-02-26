---
title: Update applyVendorEntries | Microsoft Docs
description: Updates an  apply vendor entry object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: reference
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 02/26/2021
ms.author: solsen
---

<!-- NOTE: This article is an auto-generated stub from the metadata file. -->
<!-- The sections marked with an EDIT_IS_REQUIRED require manual editing. -->
# Update applyVendorEntries

Updates the properties of an apply vendor entry object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request

Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).

```
PATCH businesscentralPrefix/companies({id})/applyVendorEntries({id})
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |
|Content-Type  |application/json|
|If-Match      |Required. When this request header is included and the eTag provided does not match the current tag on the **applyVendorEntry**, the **apply vendor entry** will not be updated. |

## Request body

In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

## Response

If successful, this method returns a ```200 OK``` response code and an updated **applyVendorEntry** object in the response body.

## Example

**Request**

Here is an example of the request.

```json
PATCH https://{businesscentralPrefix}/api/v2.0/companies({id})/applyVendorEntries({id})
Content-type: application/json
{
    "id" : "5d115c9c-44e3-ea11-bb43-000d3a2feca1",
    "applied" : true
}
```

**Response**
Here is an example of the response.


```json
HTTP/1.1 200 OK
Content-type: application/json
{
    "id" : "5d115c9c-44e3-ea11-bb43-000d3a2feca1",
    "applied" : true,
    "appliesToId" : "1e8cb9c0-44e3-ea11-bb43-000d3a2feca1",
    "postingDate" : "2020-10-05",
    "documentType" : "Invoice",
    "documentNumber" : "2001",
    "externalDocumentNumber" : "2001",
    "vendorNumber" : "10000",
    "vendorName" : "First Up Consultants",
    "description" : "",
    "remainingAmount" : 0
}
```

## See Also

[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)  
[applyVendorEntry](../resources/dynamics_applyVendorEntry.md)