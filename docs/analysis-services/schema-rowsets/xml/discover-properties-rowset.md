---
title: DISCOVER_PROPERTIES-Rowset | Microsoft Docs
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.component: schema-rowsets
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
ms.openlocfilehash: 113157cd08955aab90281ca072d98f6f68f5571a
ms.sourcegitcommit: f1caaa156db2b16e817e0a3884394e7b30fb642f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="discoverproperties-rowset"></a>DISCOVER_PROPERTIES-Rowset
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Gibt eine Liste mit Informationen und Werten zu den standardmäßigen und anwenderspezifischen Eigenschaften zurück, die vom [!INCLUDE[msCoName](../../../includes/msconame-md.md)] XMLA-Anbieter (XML for Analysis) für die angegebene Datenquelle unterstützt werden. Nicht unterstützte Eigenschaften werden nicht im zurückgegebenen Resultset aufgelistet.  
  
 Beim Aufrufen der [Discover](../../../analysis-services/xmla/xml-elements-methods-discover.md) Methode mit der **DISCOVER_PROPERTIES** Enumerationswert in der [RequestType](../../../analysis-services/xmla/xml-elements-properties/requesttype-element-xmla.md) Element, das **Discover** Methode gibt die **DISCOVER_PROPERTIES** Rowset...  
  
## <a name="rowset-columns"></a>Rowsetspalten  
 Das **DISCOVER_PROPERTIES** -Rowset enthält die folgenden Spalten.  
  
|Spaltenname|Typ|Länge|Description|  
|-----------------|----------|------------|-----------------|  
|**Eigenschaftenname**|**DBTYPE_WSTR**||Der Name der Eigenschaft.|  
|**PropertyDescription**|**DBTYPE_WSTR**||Eine lokalisierbare Textbeschreibung der Eigenschaft. Kann **NULL**zurückgeben.|  
|**PropertyType**|**DBTYPE_WSTR**||Der XML-Datentyp der Eigenschaft.<br /><br /> Kann **NULL**zurückgeben.|  
|**PropertyAccessType**|**DBTYPE_WSTR**||Der Zugriff für die Eigenschaft. Der Wert kann **Read**, **Write**oder **ReadWrite**lauten.|  
|**"IsRequired"**|**DBTYPE_BOOL**||Ein boolescher Wert, der angibt, ob eine Eigenschaft erforderlich ist.<br /><br /> True, wenn eine Eigenschaft erforderlich ist; False, wenn keine erforderlich ist.<br /><br /> Kann **NULL**zurückgeben.|  
|**Wert**|**DBTYPE_WSTR**||Der aktuelle Wert der Eigenschaft.<br /><br /> Kann **NULL**zurückgeben.|  
  
 Dieses Schemarowset ist nicht sortiert.  
  
## <a name="restriction-columns"></a>Einschränkungsspalten  
 Das **DISCOVER_PROPERTIES** -Rowset kann auf die in der folgenden Tabelle aufgeführte Spalte eingeschränkt werden.  
  
|Spaltenname|Typindikator|Einschränkungsstatus|  
|-----------------|--------------------|-----------------------|  
|**Eigenschaftenname**|**DBTYPE_WSTR**||  
  
## <a name="see-also"></a>Siehe auch  
 [XML for Analysis-Schemarowsets](../../../analysis-services/schema-rowsets/xml/xml-for-analysis-schema-rowsets.md)  
  
  
