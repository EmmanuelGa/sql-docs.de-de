---
title: DISCOVER_PARTITION_DIMENSION_STAT-Rowset | Microsoft Docs
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.component: schema-rowsets
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
ms.openlocfilehash: 1c0256dc955aa58ffd0fdd5c9176346a97b9c656
ms.sourcegitcommit: f1caaa156db2b16e817e0a3884394e7b30fb642f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="discoverpartitiondimensionstat-rowset"></a>DISCOVER_PARTITION_DIMENSION_STAT-Rowset
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Gibt Statistiken zur Dimension zurück, die einer Partition zugeordnet ist.  
  
 **Gilt für:** tabellarische und mehrdimensionale Modelle  
  
## <a name="rowset-columns"></a>Rowsetspalten  
 Das **DISCOVER_PARTITION_DIMENSION_STAT** -Rowset enthält die folgenden Spalten.  
  
|Spaltenname|Typindikator|Einschränkung|Description|  
|-----------------|--------------------|-----------------|-----------------|  
|**DATABASE_NAME**|**DBTYPE_WSTR**|Erforderlich|Der Name der Datenbank.<br /><br /> Diese Spalte ist in der Einschränkungsliste erforderlich.|  
|**CUBE_NAME**|**DBTYPE_WSTR**|Erforderlich|Der Namen des Cubes oder des Tabellenmodells.<br /><br /> Diese Spalte ist in der Einschränkungsliste erforderlich.|  
|**MEASURE_GROUP_NAME**|**DBTYPE_WSTR**|Erforderlich|Der Name der Measuregruppe.<br /><br /> Diese Spalte ist in der Einschränkungsliste erforderlich.|  
|**PARTITION_NAME**|**DBTYPE_WSTR**|Erforderlich|Der Name der Partition.<br /><br /> Diese Spalte ist in der Einschränkungsliste erforderlich.|  
|**DIMENSION_NAME**|**DBTYPE_WSTR**||Der Name der Dimension.<br /><br /> Diese Spalte ist in der Einschränkungsliste erforderlich.|  
|**ATTRIBUTE_NAME**|**DBTYPE_WSTR**||Der Name eines Attributs in der Dimension.|  
|**ATTRIBUTE_INDEXED**|**DBTYPE_BOOL**||true, um anzugeben, dass das Attribut indiziert ist; andernfalls false.|  
|**ATTRIBUTE_COUNT_MIN**|**DBTYPE_I8**||Mindestanzahl für das Attribut.|  
|**ATTRIBUTE_COUNT_MAX**|**DBTYPE_I8**||Maximale Anzahl für das Attribut.|  
  
 Dieses Schemarowset ist nicht sortiert.  
  
## <a name="using-adomdnet-to-return-the-rowset"></a>Verwenden von ADOMD.NET zum Zurückgeben des Rowsets  
 Wenn Sie Metadaten mithilfe von ADOMD.NET und des Schemarowsets abrufen, können Sie entweder die GUID verwenden oder eine Referenz für ein Schemarowsetobjekt in der GetSchemaDataSet-Methode herstellen. Weitere Informationen finden Sie unter [Working with Schema Rowsets in ADOMD.NET](../../../analysis-services/multidimensional-models-adomd-net-client/retrieving-metadata-working-with-schema-rowsets.md).  
  
 Die folgende Tabelle enthält die GUID und die Zeichenfolgenwerte, die dieses Rowset identifizieren.  
  
|Argument|Wert|  
|--------------|-----------|  
|GUID|a07ccd8e-8148-11d0-87bb-00c04fc33942|  
|ADOMDNAME|PartitionDimensionStat|  
  
## <a name="see-also"></a>Siehe auch  
 [XML for Analysis-Schemarowsets](../../../analysis-services/schema-rowsets/xml/xml-for-analysis-schema-rowsets.md)  
  
  
