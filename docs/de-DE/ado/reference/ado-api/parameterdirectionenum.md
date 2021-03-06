---
title: ParameterDirectionEnum | Microsoft Docs
ms.prod: sql
ms.prod_service: drivers
ms.service: ''
ms.component: ado
ms.technology:
- drivers
ms.custom: ''
ms.date: 01/19/2017
ms.reviewer: ''
ms.suite: sql
ms.tgt_pltfrm: ''
ms.topic: conceptual
apitype: COM
f1_keywords:
- ParameterDirectionEnum
helpviewer_keywords:
- ParameterDirectionEnum enumeration [ADO]
ms.assetid: c66aa6e6-d4f0-4f0f-9640-e08ae6cfdef3
caps.latest.revision: 11
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: ba667bc530ce0fbfda9d9d6a788809fdbf5725c5
ms.sourcegitcommit: 2ddc0bfb3ce2f2b160e3638f1c2c237a898263f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="parameterdirectionenum"></a>ParameterDirectionEnum
Gibt an, ob die [Parameter](../../../ado/reference/ado-api/parameter-object.md) stellt einen Eingabeparameter, Ausgabeparameter, sowohl ein Eingabe- und ein Output-Parameter oder den Rückgabewert einer gespeicherten Prozedur.  
  
|Konstante|Wert|Description|  
|--------------|-----------|-----------------|  
|**adParamInput**|1|Standard. Gibt an, dass der Parameter einen Eingabeparameter darstellt.|  
|**adParamInputOutput**|3|Gibt an, dass der Parameter einen Eingabe- und Parameter darstellt.|  
|**adParamOutput**|2|Gibt an, dass der Parameter einen Ausgabeparameter darstellt.|  
|**adParamReturnValue**|4|Gibt an, dass der Parameter einen Rückgabewert darstellt.|  
|**adParamUnknown**|0|Gibt an, dass die Richtung des Parameters unbekannt ist.|  
  
## <a name="adowfc-equivalent"></a>ADO/WFC-Entsprechung  
 Paket: **com.ms.wfc.data**  
  
|Konstante|  
|--------------|  
|AdoEnums.ParameterDirection.INPUT|  
|AdoEnums.ParameterDirection.INPUTOUTPUT|  
|AdoEnums.ParameterDirection.OUTPUT|  
|AdoEnums.ParameterDirection.RETURNVALUE|  
|AdoEnums.ParameterDirection.UNKNOWN|  
  
## <a name="applies-to"></a>Gilt für  
  
|||  
|-|-|  
|[CreateParameter-Methode (ADO)](../../../ado/reference/ado-api/createparameter-method-ado.md)|[Direction-Eigenschaft](../../../ado/reference/ado-api/direction-property.md)|
