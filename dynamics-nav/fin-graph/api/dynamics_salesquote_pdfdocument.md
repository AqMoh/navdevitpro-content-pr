---
title: Get pdfDocument | Microsoft Docs
description: Gets a PDF document on a salesQuote in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen

ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/28/2018
ms.author: solsen
---

# Get pdfDocument
Retrieve a PDF print-out of the corresponding document as binary content for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].


## HTTP request
The following example gets a link to the content of the PDF:

```
GET /businesscentral/api/beta/companies({id})/salesQuote({quoteId})/pdfDocument
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and a link to the PDF document in the response body.

## Example

**Request**
Here is an example of the request.

```json
GET https://api.businesscentral.dynamics.com/v1.0/api/beta/companies({id})/salesQuotes({quoteId})/pdfDocument
```

**Response**
Here is an example of the response.

> [!NOTE]  
> The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
{

    "@odata.context":"http://api.businesscentral.dynamics.com/v1.0/api/beta/$metadata#companies('CRONUS%20International%20Ltd.')/salesQuotes(94913756-80e9-47bc-995a-048a655b8cdd)/pdfDocument",
    "value":
    [
        {
            "@odata.etag":"W/\"JzQ0O0tQNUdjaUtZcU8rcUNCQTdXOUxIZVEwalA0clhjSmlXU1pqWjQ4RFczd2s9MTswMDsn\"",
            "id":"94913756-80e9-47bc-995a-048a655b8cdd",
            "content@odata.mediaReadLink":"http:// api.businesscentral.dynamics.com/v1.0/pi/beta/companies(name='CRONUS%20International%20Ltd.')/salesQuotes(94913756-80e9-47bc-995a-048a655b8cdd)/pdfDocument(94913756-80e9-47bc-995a-048a655b8cdd)/content"
        }
    ]
}
```

## HTTP request
The following example gets the actual PDF document:
`GET /businesscentral/api/beta/companies({companyid})/salesQuotes({quoteId})/pdfDocument({invoiceid})/content`

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and the PDF document in the response body.

## Example

**Request**
Here is an example of the request.

```
GET https://api.businesscentral.dynamics.com/v1.0/api/beta/companies({companyid})/salesQuotes({quoteId})/pdfDocument({id})/content
```

**Response** 
The PDF document in binary format.

## See also
[Enabling the APIs for Microsoft Dynamics NAV](../../enabling-apis-for-dynamics-nav.md)  
[Endpoints for the APIs](../../endpoints-apis-for-dynamics.md)  
[Error Codes](../dynamics_error_codes.md)  