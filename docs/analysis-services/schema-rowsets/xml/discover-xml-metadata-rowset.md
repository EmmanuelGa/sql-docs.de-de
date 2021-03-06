---
title: DISCOVER_XML_METADATA-Rowset | Microsoft Docs
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.component: schema-rowsets
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
ms.openlocfilehash: a01f73cb3ef8647f179143e4be8b71f9dceee755
ms.sourcegitcommit: f1caaa156db2b16e817e0a3884394e7b30fb642f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="discoverxmlmetadata-rowset"></a>DISCOVER_XML_METADATA-Rowset
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Gibt ein XML-Dokument zurück, in dem ein angefordertes Objekt beschrieben wird. Das zurückgegebene Rowset besteht immer aus einer Zeile und einer Spalte.  
  
 Beim Aufrufen der [Discover](../../../analysis-services/xmla/xml-elements-methods-discover.md) Methode mit der **DISCOVER_XML_METATDATA** Enumerationswert in der [RequestType](../../../analysis-services/xmla/xml-elements-properties/requesttype-element-xmla.md) Element, das **Discover**Methode gibt die **DISCOVER_XML_METATDATA** Rowset.  
  
## <a name="rowset-columns"></a>Rowsetspalten  
 Das **DISCOVER_XML_METADATA** -Rowset enthält die folgenden Spalten.  
  
|Spaltenname|Typindikator|Länge|Description|  
|-----------------|--------------------|------------|-----------------|  
|**METADATA**|**DBTYPE_WSTR**||Ein XML-Dokument, das das von der Einschränkung angeforderte Objekt beschreibt.|  
  
 Dieses Schemarowset ist nicht sortiert.  
  
> [!IMPORTANT]  
>  Das **DISCOVER_XML_METADATA** -Rowset kann nicht mithilfe der SELECT-Befehlssyntax abgefragt werden. Allerdings die **DISCOVER_XML_METADATA** Rowset kann abgefragt werden, mithilfe von <xref:Microsoft.AnalysisServices.AdomdClient.AdomdConnection.GetSchemaDataSet%2A>.  
  
## <a name="restriction-columns"></a>Einschränkungsspalten  
 Das **DISCOVER_XML_METADATA** -Rowset kann auf die in der folgenden Tabelle aufgeführten Spalten eingeschränkt werden.  
  
|Spaltenname|Typindikator|Einschränkungsstatus|  
|-----------------|--------------------|-----------------------|  
|**DatabaseID**|**DBTYPE_WSTR**|Optional.|  
|**DimensionID**|**DBTYPE_WSTR**|Optional.|  
|**CubeID**|**DBTYPE_WSTR**|Optional.|  
|**MeasureGroupID**|**DBTYPE_WSTR**|Optional.|  
|**PartitionID**|**DBTYPE_WSTR**|Optional.|  
|**PerspectiveID**|**DBTYPE_WSTR**|Optional.|  
|**DimensionPermissionID**|**DBTYPE_WSTR**|Optional.|  
|**RoleID-Wert**|**DBTYPE_WSTR**|Optional.|  
|**DatabasePermissionID**|**DBTYPE_WSTR**|Optional.|  
|**MiningModelID**|**DBTYPE_WSTR**|Optional.|  
|**MiningModelPermissionID**|**DBTYPE_WSTR**|Optional.|  
|**DataSourceID-Wert**|**DBTYPE_WSTR**|Optional.|  
|**MiningStructureID**|**DBTYPE_WSTR**|Optional.|  
|**AggregationDesignID**|**DBTYPE_WSTR**|Optional.|  
|**TraceID**|**DBTYPE_WSTR**|Optional.|  
|**MiningStructurePermissionID**|**DBTYPE_WSTR**|Optional.|  
|**CubePermissionID**|**DBTYPE_WSTR**|Optional.|  
|**AssemblyID**|**DBTYPE_WSTR**|Optional.|  
|**MdxScriptID**|**DBTYPE_WSTR**|Optional.|  
|**DataSourceViewID**|**DBTYPE_WSTR**|Optional.|  
|**DataSourcePermissionID**|**DBTYPE_WSTR**|Optional.|  
|**ObjectExpansion**|**DBTYPE_WSTR**|Optional.|  
  
 Die Einschränkung **ObjectExpansion**, steht für jedes Hauptobjekt von [!INCLUDE[msCoName](../../../includes/msconame-md.md)] [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] [!INCLUDE[ssASnoversion](../../../includes/ssasnoversion-md.md)]. Der Client verwendet normalerweise Einschränkungen, um die OLAP-Objekte zu beschreiben, für die der DDL-Code zurückgegeben wird, und er verwendet die **ObjectExpansion** -Einschränkung, um den Grad der Erweiterung im zurückgegebenen DDL-Code zu definieren. In der folgenden Tabelle angibt, ob der Enumerationswert für [Element Alter &#40;XMLA&#41; ](../../../analysis-services/xmla/xml-elements-commands/alter-element-xmla.md) Befehle.  
  
|Enumerationswert|Description|  
|-----------------------|-----------------|  
|**ReferenceOnly**|Gibt nur den angeforderten Namen, den Timestamp, die ID und den Status für das angeforderte Objekt und alle nachfolgenden Hauptobjekte rekursiv zurück.|  
|**' ObjectProperties '**|Erweitert das angeforderte Objekt ohne Verweise auf enthaltene Objekte (schließt enthaltene erweiterte Nebenobjekte ein).|  
|**' ExpandObject '**|Wie *ObjectProperties*, gibt jedoch auch den Namen, die ID und den Timestamp für enthaltene Hauptobjekte zurück.|  
|**ExpandFull**|Erweitert das angeforderte Objekt vollständig rekursiv bis zum Ende eines jeden enthaltenen Objekts.|  
  
## <a name="see-also"></a>Siehe auch  
 [XML for Analysis-Schemarowsets](../../../analysis-services/schema-rowsets/xml/xml-for-analysis-schema-rowsets.md)  
  
  
