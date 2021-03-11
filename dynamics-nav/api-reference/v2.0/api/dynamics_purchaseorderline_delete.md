---
title: Delete purchaseOrderLine | Microsoft Docs
description: Deletes a purchase order line object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 02/24/2021
ms.author: solsen
---

<!-- NOTE: This article is an auto-generated stub from the metadata file. -->
<!-- The sections marked with an EDIT_IS_REQUIRED require manual editing. -->
# Delete purchaseOrderLine

Deletes a purchase order line from [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request

Replaces the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).

```
DELETE businesscentralPrefix/companies({id})/purchaseOrders({id})/purchaseOrderLines({purchaseOrderLineId})
DELETE businesscentralPrefix/companies({id})/purchaseOrderLines({purchaseOrderLineId})
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |
|If-Match       |Required. When this request header is included and the eTag provided does not match the current tag on the **purchaseOrderLine**, the **purchaseOrderLine** will not be updated. |


## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns ```204 No Content``` response code and deletes the purchaseOrderLine. It does not return anything in the response body.

## Example

**Request**

Here is an example of the request.

```json
DELETE https://{businesscentralPrefix}/api/v2.0/companies({id})/purchaseOrderLines({purchaseOrderLineId})
```

**Response**

Here is an example of the response.

```json
HTTP/1.1 204 No Content
```

## See Also

[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)  
[purchaseOrderLine](../resources/dynamics_purchaseOrderLine.md)  
[GET purchaseOrderLine](dynamics_purchaseorderline_get.md)  
[POST purchaseOrderLine](dynamics_purchaseorderline_create.md)  
[PATCH purchaseOrderLine](dynamics_purchaseorderline_update.md)  
