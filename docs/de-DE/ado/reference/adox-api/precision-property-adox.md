---
title: Precision-Eigenschaft (ADOX) | Microsoft Docs
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
- _Column::put_Precision
- _Column::PutPrecision
- _Column::GetPrecision
- _Column::get_Precision
- _Column::Precision
helpviewer_keywords:
- Precision property [ADOX]
ms.assetid: 0e0ecbbf-d7de-49d4-a128-5a519ecd54ba
caps.latest.revision: 11
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 73ea0021a6cb74fb7e3e98009be3566270d783e9
ms.sourcegitcommit: 2ddc0bfb3ce2f2b160e3638f1c2c237a898263f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="precision-property-adox"></a>Precision-Eigenschaft (ADOX)
Gibt die maximale Genauigkeit von Datenwerten in den [Spalte](../../../ado/reference/adox-api/column-object-adox.md).  
  
## <a name="settings-and-return-values"></a>Einstellungen und Rückgabewerte  
 Legt fest, und gibt eine **lange** Wert, der die maximale Genauigkeit der Datenwerte in der Spalte ist bei der [Typ](../../../ado/reference/adox-api/type-property-column-adox.md) Eigenschaft ist ein numerischer Typ. **Genauigkeit** wird für alle anderen Datentypen ignoriert.  
  
## <a name="remarks"></a>Hinweise  
 Der Standardwert ist 0 (null) (**0**).  
  
 Diese Eigenschaft ist schreibgeschützt und für [Spalte](../../../ado/reference/adox-api/column-object-adox.md) Objekte, die bereits an eine Auflistung angefügt.  
  
## <a name="applies-to"></a>Gilt für  
 [Column-Objekt (ADOX)](../../../ado/reference/adox-api/column-object-adox.md)  
  
## <a name="see-also"></a>Siehe auch  
 [ADOX-Codebeispiel: NumericScale und Genauigkeit Eigenschaften-Beispiel (VB)](../../../ado/reference/adox-api/adox-code-example-numericscale-and-precision-properties-example-vb.md)   
 [Type-Eigenschaft (Spalte) (ADOX)](../../../ado/reference/adox-api/type-property-column-adox.md)   
 [Column-Objekt (ADOX)](../../../ado/reference/adox-api/column-object-adox.md)
