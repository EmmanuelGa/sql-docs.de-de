---
title: AggregationDesign-Element (ASSL) | Microsoft Docs
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.component: assl
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
ms.openlocfilehash: da7013f6e6b3e35ebf58b35c902471b8f86076d0
ms.sourcegitcommit: f1caaa156db2b16e817e0a3884394e7b30fb642f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="aggregationdesign-element-assl"></a>AggregationDesign-Element (ASSL)
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Definiert einen Satz von Aggregationsdefinitionen, die für mehrere Partitionen in einer Datenbank freigegeben sein können.  
  
## <a name="syntax"></a>Syntax  
  
```xml  
  
<AggregationDesigns>  
   <AggregationDesign>  
      <ID>...</ID>  
      <Name>...</Name>  
            <Description>...</Description>  
      <EstimatedRows>...</EstimatedRows>  
      <Dimensions>...</Dimensions>  
            <Aggregations>...</Aggregation>  
      <EstimatedPerformanceGain>...</EstimatedPerformanceGain>  
      <Annotations>...</Annotations>  
   </AggregationDesign>  
</AggregationDesigns>  
```  
  
## <a name="element-characteristics"></a>Elementmerkmale  
  
|Merkmal|Beschreibung|  
|--------------------|-----------------|  
|Datentyp und -länge|Keine|  
|Standardwert|Keine|  
|Kardinalität|0-n: Optionales Element, das mehr als einmal auftreten kann.|  
  
## <a name="element-relationships"></a>Elementbeziehungen  
  
|Beziehung|Element|  
|------------------|-------------|  
|Übergeordnete Elemente|[AggregationDesigns](../../../analysis-services/scripting/collections/aggregationdesigns-element-assl.md)|  
|Untergeordnete Elemente|[Aggregationen](../../../analysis-services/scripting/collections/aggregations-element-assl.md), [Anmerkungen](../../../analysis-services/scripting/collections/annotations-element-assl.md), [Beschreibung](../../../analysis-services/scripting/properties/description-element-assl.md), [Dimensionen](../../../analysis-services/scripting/collections/dimensions-element-assl.md), [EstimatedPerformanceGain](../../../analysis-services/scripting/properties/estimatedperformancegain-element-assl.md), [EstimatedRows](../../../analysis-services/scripting/properties/estimatedrows-element-assl.md), [ID](../../../analysis-services/scripting/properties/id-element-assl.md), [Name](../../../analysis-services/scripting/properties/name-element-assl.md)|  
  
## <a name="remarks"></a>Hinweise  
 Das entsprechende Element im Objektmodell von Analysis Management Objects (AMO) ist <xref:Microsoft.AnalysisServices.AggregationDesign>.  
  
## <a name="see-also"></a>Siehe auch  
 [Partitions-Element &#40;ASSL&#41;](../../../analysis-services/scripting/objects/partition-element-assl.md)   
 [Aggregation-Element & #40; ASSL & #41;](../../../analysis-services/scripting/objects/aggregation-element-assl.md)   
 [Aggregations-Element &#40;ASSL&#41;](../../../analysis-services/scripting/collections/aggregations-element-assl.md)   
 [Objekte & #40; ASSL & #41;](../../../analysis-services/scripting/objects/objects-assl.md)  
  
  
