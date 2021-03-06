---
title: "DISCOVER_TRACES Rowset | Microsoft Docs"
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.custom: schema-rowsets
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
---
# DISCOVER_TRACES Rowset
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Provides information about traces that are currently active on the server.  
  
 **Applies to:** tabular models, multidimensional models  
  
## Rowset Columns  
 The **DISCOVER_TRACES** rowset contains the following columns.  
  
|Column name|Type indicator|Description|  
|-----------------|--------------------|-----------------|  
|**TraceID**|**DBTYPE_WSTR**|The trace ID.|  
|**TraceName**|**DBTYPE_WSTR**|The trace name.|  
|**LogFileName**|**DBTYPE_WSTR**|The trace log file name.|  
|**LogFileSize**|**DBTYPE_I4**|The trace log file size.|  
|**LogFileRollover**|**DBTYPE_BOOL**|When true, indicates that the log file should be rolled over; otherwise false.|  
|**AutoRestart**|**DBTYPE_BOOL**|When true, indicates that the auto restart option is enabled; otherwise false.|  
|**CreationTime**|**DBTYPE_TIME**|The date and time that the trace was created.|  
|**StopTime**|**DBTYPE_TIME**|The stop time of a trace.|  
|**Type**|**PF_DBTYPE_WSTR**|The type of trace.|  
  
 This schema rowset is not sorted.  
  
## Restriction Columns  
 The **DISCOVER_TRACES** rowset can be restricted on the columns listed in the following table.  
  
|Column name|Type indicator|Restriction State|  
|-----------------|--------------------|-----------------------|  
|**TraceId**|**DBTYPE_I4**|Optional.|  
|**Type**|WSTR|Optional.|  
  
## Using ADOMD.NET to return the rowset  
 When using ADOMD.NET and the schema rowset to retrieve metadata, you can use either the GUID or string to reference a schema rowset object in the GetSchemaDataSet method. For more information, see [Working with Schema Rowsets in ADOMD.NET](../../../analysis-services/multidimensional-models-adomd-net-client/retrieving-metadata-working-with-schema-rowsets.md).  
  
 The following table provides the GUID and string values that identify this rowset.  
  
|Argument|Value|  
|--------------|-----------|  
|GUID|a07ccd1a-8148-11d0-87bb-00c04fc33942|  
|String|DISCOVER_TRACES|  
  
## See Also  
 [XML for Analysis Schema Rowsets](../../../analysis-services/schema-rowsets/xml/xml-for-analysis-schema-rowsets.md)  
  
  
