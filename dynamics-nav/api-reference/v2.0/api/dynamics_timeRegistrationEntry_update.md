---
title: Patch timeRegistrationEntries| Microsoft Docs
description: Patch a timeRegistrationEntries in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2019
ms.author: solsen
---

# Update timeRegistrationEntries
Update a timeRegistrationEntry in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].


## HTTP request
Replace the URL prefix for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] depending on environment following the [guideline](../../v2.0/endpoints-apis-for-dynamics.md).
```
PATCH businesscentralPrefix/companies({companyId})/timeRegistrationEntries({timeregistrationId})
```

## Request headers

|Header        |Value                    |
|--------------|-------------------------|
|Authorization |Bearer {token}. Required.|
|Content-Type  |application/json         |
|If-Match  |*application/json*         |


## Example

**Request**

Here is an example of the request.
```json
PATCH https://{businesscentralPrefix}/api/v2.0/companies({id})/timeRegistrationEntries({timeregistrationId})
Content-type: application/json

{
	"quantity": 8
}
```

**Response**

Here is an example of the response. 

> [!NOTE]  
>   The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "1a8b1fec-c0e3-ea11-aa60-000d3ad7cacb",
    "employeeId": "258bb9c0-44e3-ea11-bb43-000d3a2feca1",
    "employeeNumber": "AH",
    "jobId": "00000000-0000-0000-0000-000000000000",
    "jobNumber": "",
    "jobTaskNumber": "",
    "absence": "",
    "lineNumber": 10000,
    "date": "2019-02-02",
    "quantity": 8,
    "status": "Open",
    "unitOfMeasureId": "56a6738a-44e3-ea11-bb43-000d3a2feca1",
    "unitOfMeasureCode": "HOUR",
    "lastModfiedDateTime": "2020-08-21T15:13:58.87Z"
```

## See also
[Tips for working with the APIs](/dynamics365/business-central/dev-itpro/developer/devenv-connect-apps-tips)  
[Error Codes](../dynamics_error_codes.md)  
[timeRegistrationEntries](../resources/dynamics_timeRegistrationEntry.md)  
[Get timeRegistrationEntries](../api/dynamics_timeRegistrationEntry_get.md)  
[Post timeRegistrationEntries](../api/dynamics_timeRegistrationEntry_create.md)  
[Patch timeRegistrationEntries](../api/dynamics_timeRegistrationEntry_update.md)  
[Delete timeRegistrationEntries](../api/dynamics_timeRegistrationEntry_delete.md)  
