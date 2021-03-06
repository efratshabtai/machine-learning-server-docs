--- 
 
# required metadata 
title: "rxGetVarNames function (RevoScaleR) " 
description: " Read the variable names for data source or data frame " 
keywords: "(RevoScaleR), rxGetVarNames, attribute" 
author: "heidisteen" 
manager: "jhubbard" 
ms.date: "09/07/2017" 
ms.topic: "reference" 
ms.prod: "microsoft-r" 
ms.service: "" 
ms.assetid: "" 
 
# optional metadata 
ROBOTS: "" 
audience: "" 
ms.devlang: "" 
ms.reviewer: "" 
ms.suite: "" 
ms.tgt_pltfrm: "" 
ms.technology: "r-server" 
ms.custom: "" 
 
--- 
 
 
 #rxGetVarNames: Variable names for a data source or data frame 
 ##Description
 
Read the variable names for data source or data frame
 
 
 ##Usage

```   
  rxGetVarNames(data)
 
```
 
 ##Arguments

   
    
 ### `data`
 an `RxDataSource` object, a character string specifying the .xdf file, or a data frame. 
  
 
 
 ##Details
 
If colInfo is used in the data source to specify new column names, these new
names will be used in the return value.
 
 
 ##Value
 
character vector containing the names of the variables in the data source or data frame.
 

 
 
 
 ##See Also
 
[rxGetVarInfo](rxGetVarInfoXdf.md),
[rxSetVarInfo](rxSetVarInfoXdf.md),
[rxDataStep](rxDataStep.md),
[rxGetInfo](rxGetInfoXdf.md).
   
 ##Examples

 ```
   
  # Specify name and location of sample data file
  censusWorkers <- file.path(rxGetOption("sampleDataDir"), "CensusWorkers")
  
  # Get the variable names
  varNames <- rxGetVarNames(censusWorkers)
  
  # Print the variable names
  varNames
  
 
```
 
 
