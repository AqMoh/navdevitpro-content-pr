---
title: Get customerPayments | Microsoft Docs
description: Gets a customer payment object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# Get customerPayments
Retrieve the properties and relationships of a customer payment object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).

```
GET businesscentralPrefix/companies({id})/customerPaymentsJournals({id})/customerPayments({id})
GET businesscentralPrefix/companies({id})/customerPayments({id})
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and a **customerPayments** object in the response body.

## Example

**Request**

Here is an example of the request.
```json
GET https://{businesscentralPrefix}/api/v2.0/companies({id})/customerPaymentsJournals({id})/customerPayments({id})
```

**Response**

Here is an example of the response. 


```json
{
    "id": "17cce948-c6a5-4861-8ff5-30428ed83207",
    "lineNumber": 10000,
    "customerId": "customerId-value",
    "customerNumber": "10400",
    "contactId": "string",
    "postingDate": "2015-12-31",
    "documentNumber": "1234",
    "externalDocumentNumber": "",
    "amount": 1500,
    "appliesToInvoiceId": "appliesToInvoiceId-value",
    "appliesToInvoiceNumber": "100000",
    "description": "",
    "comment": "",
    "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)
[customerpayment](../resources/dynamics_customerpayment.md)[Delete customerpayment](../api/dynamics_customerpayment_Delete.md)
[Create customerpayment](../api/dynamics_customerpayment_Create.md)
[Update customerpayment](../api/dynamics_customerpayment_Update.md)
