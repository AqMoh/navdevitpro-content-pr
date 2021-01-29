---
title: UK Features that are Moved, Removed, or Replaced | Microsoft Docs
description: We are constantly streamlining and adjusting our app in-step with market developments. Read about the features for the UK that we have moved, removed, or replaced.
author: bholtorf

ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: deprecated, United Kingdom, local functionality
ms.date: 08/23/2018
ms.author: bholtorf

---

# Deprecated Features in the UK Version of Microsoft Dynamics NAV 2018
This topic lists and describes the local functionality for the United Kingdom that has been removed from [!INCLUDE[navnow](includes/navnow_md.md)], made available from a new page or report, or replaced by a new feature.

## Localize Intrastat Reporting
You must report shipment method during Intrastat reporting to be legally compliant. The code for the shipment method must be transferred from the Intrastat journal.

|Moved, Removed, or Replaced?| Why?|
|----|----|
| Replaced | The Localize Intrastat Reporting feature has been replaced with the **Shipment Method Mandatory** field in the **Intrastat Setup** window in the standard product.|

## Accounting Periods and System Calendar
If your fiscal year is different than the calendar, you can measure your fiscal period in other units of time, such as months or quarters. To do this, you set up system calendars and accounting periods.

|Moved, Removed, or Replaced?| Why?|
|----|----|
| Removed | Lack of use. Additionally, there are standard features for accounting periods that provide most of the same functionality as the UK accounting periods. |

## Create and Export a Bankers' Automated Clearing Service File
You can use Bankers' Automated Clearing Service (BACS) to process financial transactions electronically. To do so, you must export vendor payments to a BACS file using the Export BACS option.

|Moved, Removed, or Replaced?| Why?|
|----|----|
| Removed | This banking format standard is no longer used. This functionality is now covered by extensions such as the Envestnet Yodlee Bank Feeds, AMC Banking, and various other formats. |

<!-- THIS WORK DID NOT GET DONE. EXPECT IT TO COME IN A FUTURE UPDATE
## Multiple interest rates
To let you use more than one interest rate to calculate finance charges for a specific period, you can specify multiple rates for each finance charge term.

|Moved, Removed, or Replaced?|Why?|
|----|----|
|Moved| This functionality is also available to countries such as NO, SE, FI, and IT, so we have removed the country-specific designation so that it's available to everyone.|
-->

<!-- THIS WORK DID NOT GET DONE. EXPECT IT TO COME IN A FUTURE UPDATE
## VAT Audit reports
VAT Audit reports let you generate VAT amounts for a specific period in response to an audit from a tax authority:

* **VAT Audit** - Used for VAT auditing.
* **VAT Entry Exception** - Details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts. It also displays the difference in VAT amounts for the tax authorities.

|||
|----|----|
|Moved, Removed, or Replaced?| Why?|
|Replaced| The VAT Audit report is replaced. Now you can export data to Excel through the OData service. The VAT Entry Exception report is no longer specific to the UK. The documentation for these reports has moved to the [!INCLUDE[d365fin](includes/d365fin_md.md)] repository.|
-->

## Non-Invoiced Stock Reports
For month-end reconciliation and auditing, you can use the **Stock Received Not Invoiced** report to view stock that is received but not yet invoiced, and the **Stock Shipped Not Invoiced** report to see stock that has been shipped but not yet invoiced.

|Moved, Removed, or Replaced?|Why?|
|----|----|
|Moved | The functionality for the Shipped, Non-Invoiced Sales Orders and the Received, Not Invoiced Purchase Order reports are no longer specific to the UK, so we have made them generally available as views for sales orders and purchase orders. The views are available in the Navigation Pane as Shipped Not Invoiced and Shipped Not Received options under Sales Orders and Purchase Orders, respectively.|

### Print Unposted Sales and Unposted Purchase Reports
The Unposted Sales and Unposted Purchase reports let you print a list of sales and purchase documents that are not yet posted.  

|Moved, Removed, or Replaced?| Why?|
|----|----|
| Moved | The Unposted Sales and Unposted Purchase reports are now available from the Navigation Pane as views under Sales Orders and Purchase Orders. |

### Other VAT Reports
You can use the following reports for VAT reporting:  

* **Day Book VAT Entry** - Displays the daily total for VAT entries for a specific period.
* **Day Book Cust. Ledger Entry** - Displays the daily total for customer ledger entries for a specific period.
* **Day Book Vendor Ledger Entry** - Displays the daily total for vendor ledger entries for a specific period.

|Moved, Removed, or Replaced?|Why?|
|----|----|
|Moved| These VAT-related reports are no longer specific to the UK, so we have made them generally available in the standard product.  |

## Specify the Supply Type on Documents
You can specify supply types such as sales, loan, exchange, hire, lease, rental, sales on commission, on tax invoices. To do this, you must update the codes and names of the supply types in the **Types of Supply** window.

|Moved, Removed, or Replaced?|Why?|
|----|----|
|Removed| Lack of use. The business need that this functionality was introduced to cover is no longer relevant.  |

## Multiple Interest Rates
When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods.

|Moved, Removed, or Replaced?|Why?|
|----|----|
|Moved| The Multiple Interest Rates feature is no longer specific to the UK, so we have made it generally available in the standard product. |

## Objects or Fields Deleted in [!INCLUDE[nav2018](includes/nav2018_md.md)]
The following list shows fields that are deleted as a result of removed features.  

|Table ID|Table Name|Field ID|Field Name|
|--------|--------|----------|-----------|
|23|Vendor|10550|BACS Account No.|
|81|Gen. Journal Line|10550|BACS Account No.|
|81|Gen. Journal Line|10551|BACS Exported|
|81|Gen. Journal Line|10552|BACS Entry No.|
|81|Gen. Journal Line|10553|Recurring Calendar Source|
|263|Intrastat Jnl. Line|10500|Shipment Method|
|271|Bank Account Ledger Entry|10550|BACS Ledger Entries|
|312|Purchases & Payables Setup|10550|BACS File Name|
|312|Purchases & Payables Setup|10551|Import BACS Files|
|334|Column Layout|10505|Keep Comparison Period Scope|
|363|Analysis View|10550|Calendar Source|
|7118|Analysis Column|10505|Keep Comparison Period Scope|
|7152|Item Analysis View|10550|Calendar Source|

## See Also
[Upgrading to Microsoft Dynamics NAV 2018](upgrading-to-microsoft-dynamics-nav.md)  
[Upgrading the Application Code](upgrading-the-application-code.md)  
[Deprecated Fields, and Fields Marked as Obsolete](deprecated-fields.md)  
[United Kingdom Local Functionality in [!INCLUDE[navnow](includes/navnow_md.md)]](/dynamics-nav-app/LocalFunctionality/unitedkingdom/united-kingdom-local-functionality)  
