---
title: "FIELDERROR Function (Record)"
description: FIELDERROR Function (Record)
ms.custom: na
ms.date: 06/05/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
ms.assetid: 5a713a53-3902-40e9-a0fb-e1a9ba1ac420
caps.latest.revision: 11
manager: edupont
---
# FIELDERROR Function (Record)
Stops the execution of the code causing a run-time error, and creates an error message for a field.  
  
## Syntax  
  
```  
  
Record.FIELDERROR(Field, [Text])  
```  
  
#### Parameters  
 *Record*  
 Type: Record  
  
 The record that contains the field.  
  
 *Field*  
 Type: Field  
  
 The field for which you want to create an error message.  
  
 *Text*  
 Type: Text or code  
  
 Use this optional parameter to include the text of the error message. If you do not use this parameter, then default text is used as shown in the following examples. You can use backslashes \(\\\) to break lines.  
  
## Remarks  
 Like a run-time error, this function causes the system to automatically abort any transaction.  
  
## Programming Guidelines  
 We recommend the following guidelines for error messages:  
  
- Describe what is wrong and how to solve the problem.  
  
- Write a short descriptive message. Do not use more words than necessary.  
  
- Note that a period is automatically inserted at the end of a FIELDERROR.  
  
- Use a text constant for the *Text* parameter.  
  
  For more information, see [Progress Windows, MESSAGE, ERROR, and CONFIRM Functions](Progress-Windows--MESSAGE--ERROR--and-CONFIRM-Functions.md).  
  
## Example 1 
 In the first example, there is no *Text* parameter and the field does not have a value. This example requires that you create a Record variable for the **Customer** table named CustomerRec.  
  
```  
CustomerRec."No." := '';  
CustomerRec.FIELDERROR("No.");  
```  
  
 The following message is displayed:  
  
 **You must specify No. in Customer No.=''.**  
  
## Example 2 
 In the next example, there is no *Text* parameter and the field has a value. This example requires that you create a Record variable for the **Customer** table named CustomerRec.  
  
```  
CustomerRec."No." := 'NEW 3500';  
CustomerRec.FIELDERROR("No.");  
```  
  
 The following message is displayed:  
  
 **No. must not be NEW 3500 in Customer No.='NEW 3500'.**  
  
## Example 3 
 The third example uses a non-empty string as the *Text* parameter. This example requires that you create the following variables and text constant in the **C/AL Globals** window.  
  
|Variable name|DataType|Subtype|  
|-------------------|--------------|-------------|  
|CustomerRec|Record|Customer|  
  
|Text constant name|ConstValue|  
|------------------------|----------------|  
|Text001|is not valid|  
  
```  
CustomerRec."No." := 'NEW 3500';  
CustomerRec.FIELDERROR("No.", Text001);  
```  
  
 The following message is displayed:  
  
 **No. is not valid in Customer No.='NEW 3500'.**  
  
## See Also  
 [Record Data Type](Record-Data-Type.md)