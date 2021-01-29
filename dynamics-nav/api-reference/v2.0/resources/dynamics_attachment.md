---
title: attachment resource type | Microsoft Docs
description: An attachments object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 01/29/2021
ms.author: solsen
---

<!-- START>DO_NOT_EDIT -->
<!-- IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT. -->
# attachment resource type

[!INCLUDE[api_v2_note](../../includes/api_v2_note.md)]

Represents an attachments in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods

| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET attachment](../api/dynamics_attachment_Get.md)|attachment|Gets a attachments object.|
|[DELETE attachment](../api/dynamics_attachment_Delete.md)|none|Deletes a attachments object.|
|[POST attachment](../api/dynamics_attachment_Create.md)|attachment|Creates a attachments object.|
|[PATCH attachment](../api/dynamics_attachment_Update.md)|attachment|Updates a attachments object.|


## Navigation

| Navigation |Return Type| Description |
|:----------|:----------|:-----------------|
|[salesInvoice](dynamics_salesinvoice.md)|salesInvoice |Gets the salesinvoice of the attachment.|
|[journalLine](dynamics_journalline.md)|journalLine |Gets the journalline of the attachment.|
|[generalLedgerEntry](dynamics_generalledgerentry.md)|generalLedgerEntry |Gets the generalledgerentry of the attachment.|
|[salesOrder](dynamics_salesorder.md)|salesOrder |Gets the salesorder of the attachment.|
|[salesQuote](dynamics_salesquote.md)|salesQuote |Gets the salesquote of the attachment.|
|[salesCreditMemo](dynamics_salescreditmemo.md)|salesCreditMemo |Gets the salescreditmemo of the attachment.|
|[purchaseInvoice](dynamics_purchaseinvoice.md)|purchaseInvoice |Gets the purchaseinvoice of the attachment.|

## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|parentId|GUID|The ID of the parent entity. |
|fileName|string|Logical filename.|
|byteSize|integer|File size.|
|attachmentContent|stream|The attachment's content.|
|lastModifiedDateTime|datetime|The last datetime the attachments was modified. Read-Only.|
|parentType|NAV.attachmentEntityBufferDocumentType|The type of the parent document of the attachments. It can be " ", "Journal", "Sales Order", "Sales Quote", "Sales Credit Memo", "Sales Invoice" or "Purchase Invoice".|

## JSON representation

Here is a JSON representation of the attachment resource.


```json
{
    "id": "GUID",
    "parentId": "GUID",
    "fileName": "string",
    "byteSize": "integer",
    "attachmentContent": "stream",
    "lastModifiedDateTime": "datetime",
    "parentType": "NAV.attachmentEntityBufferDocumentType"
}
```
<!-- IMPORTANT: END>DO_NOT_EDIT -->


## See Also
[GET attachment](../api/dynamics_attachment_Get.md)
[DELETE attachment](../api/dynamics_attachment_Delete.md)
[POST attachment](../api/dynamics_attachment_Create.md)
[PATCH attachment](../api/dynamics_attachment_Update.md)
