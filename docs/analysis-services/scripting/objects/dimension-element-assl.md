---
title: Dimension-Element (ASSL) | Microsoft Docs
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.component: assl
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
ms.openlocfilehash: 0db9a8565b7e82056fc102783266335a6837c3ff
ms.sourcegitcommit: f1caaa156db2b16e817e0a3884394e7b30fb642f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="dimension-element-assl"></a>Dimension-Element (ASSL)
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Definiert eine Dimension.  
  
## <a name="syntax"></a>Syntax  
  
```xml  
  
<Dimensions>  
   <Dimension xsi:type="Dimension">...</Dimension> <!-- ancestor: Database -->  
   <!-- or -->  
   <Dimension xsi:type="AggregationDimension">...</Dimension> <!-- ancestor: Aggregation -->  
   <!-- or -->  
   <Dimension xsi:type="AggregationDesignDimension">...</Dimension> <!-- ancestor: AggregationDesign -->  
   <!-- or -->  
   <Dimension xsi:type="AggregationInstanceCubeDimension">...</Dimension> <!-- ancestor: AggregationInstance -->  
      <!-- or -->  
   <Dimension xsi:type="CubeDimension">...</Dimension> <!-- ancestor: Cube -->  
      <!-- or -->  
   <Dimension xsi:type="MeasureGroupDimension">...</Dimension> <!-- ancestor: MeasureGroup -->  
   <!-- or -->  
   <Dimension xsi:type="PerspectiveDimension">...</Dimension> <!-- ancestor: Perspective -->  
</Dimensions>  
```  
  
## <a name="element-characteristics"></a>Elementmerkmale  
  
|Merkmal|Beschreibung|  
|--------------------|-----------------|  
|Datentyp und -länge|Siehe Tabelle unten.|  
|Standardwert|Keine|  
|Kardinalität|0-n: Optionales Element, das mehr als einmal auftreten kann.|  
  
|Vorgänger oder übergeordnetes Element|Datentyp|  
|------------------------|---------------|  
|[Datenbank](../../../analysis-services/scripting/objects/database-element-assl.md)|[Dimension](../../../analysis-services/scripting/data-type/dimension-data-type-assl.md)|  
|[Aggregation](../../../analysis-services/scripting/objects/aggregation-element-assl.md)|[AggregationDimension](../../../analysis-services/scripting/data-type/aggregationdimension-data-type-assl.md)|  
|[AggregationDesign](../../../analysis-services/scripting/objects/aggregationdesign-element-assl.md)|[AggregationDesignDimension](../../../analysis-services/scripting/data-type/aggregationdesigndimension-data-type-assl.md)|  
|[AggregationInstance](../../../analysis-services/scripting/objects/aggregationinstance-element-assl.md)|[AggregationInstanceCubeDimension](../../../analysis-services/scripting/data-type/aggregationinstancecubedimension-data-type-assl.md)|  
|[Cube](../../../analysis-services/scripting/objects/cube-element-assl.md)|[CubeDimension](../../../analysis-services/scripting/data-type/cubedimension-data-type-assl.md)|  
|[MeasureGroup-Objekt](../../../analysis-services/scripting/objects/measuregroup-element-assl.md)|[MeasureGroupDimension](../../../analysis-services/scripting/data-type/measuregroupdimension-data-type-assl.md)|  
|[Perspektive](../../../analysis-services/scripting/objects/perspective-element-assl.md)|[PerspectiveDimension](../../../analysis-services/scripting/data-type/perspectivedimension-data-type-assl.md)|  
  
## <a name="element-relationships"></a>Elementbeziehungen  
  
|Beziehung|Element|  
|------------------|-------------|  
|Übergeordnete Elemente|[Dimensionen](../../../analysis-services/scripting/collections/dimensions-element-assl.md)|  
|Untergeordnete Elemente|Keine|  
  
## <a name="remarks"></a>Hinweise  
 Die entsprechenden Elemente im Objektmodell von Analysis Management Objects (AMO) sind <xref:Microsoft.AnalysisServices.Dimension>, <xref:Microsoft.AnalysisServices.AggregationDimension>, <xref:Microsoft.AnalysisServices.AggregationDesignDimension>, <xref:Microsoft.AnalysisServices.CubeDimension>, <xref:Microsoft.AnalysisServices.MeasureGroupDimension>, und <xref:Microsoft.AnalysisServices.PerspectiveDimension>.  
  
## <a name="see-also"></a>Siehe auch  
 [Objekte & #40; ASSL & #41;](../../../analysis-services/scripting/objects/objects-assl.md)  
  
  
