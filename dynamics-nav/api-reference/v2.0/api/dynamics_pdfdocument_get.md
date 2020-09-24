---
title: GET pdfDocuments | Microsoft Docs
description: Gets a pdfDocument object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get pdfDocuments
Retrieve the properties and relationships of a pdfDocument object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)]. 


## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).

```
GET businesscentralPrefix/companies({id})/salesInvoices({id})/pdfDocument
GET businesscentralPrefix/companies({id})/salesQuote({id})/pdfDocument
GET businesscentralPrefix/companies({id})/salesCreditMemo({id})/pdfDocument
GET businesscentralPrefix/companies({id})/purchaseInvoice({id})/pdfDocument
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and an **pdfDocuments** object in the response body.

## Example

**Request**

Here is an example of the request.
```json
GET https://{businesscentralPrefix}/api/v2.0/companies({id})/salesInvoices({id})/pdfDocument
```

**Response**

Here is an example of the response. 

```json
{
    "id": "5fd8a1c5-bde4-ea11-bbf2-00155df3a615",
    "parentId": "5fd8a1c5-bde4-ea11-bbf2-00155df3a615",
    "parentType": "Sales Invoice", 
    "pdfDocumentContent@odata.mediaReadLink": "http://onbuyuka-azvm1.europe.corp.microsoft.com:7047/Navision_NAV/api/v2.0/companies(52e03390-bde4-ea11-bbf2-00155df3a615)/salesInvoices(5fd8a1c5-bde4-ea11-bbf2-00155df3a615)/pdfDocument/pdfDocumentContent"
}
```


## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)    
[pdfdocument](../resources/dynamics_pdfdocument.md)    
