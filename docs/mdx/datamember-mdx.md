---
title: DataMember (MDX) | Microsoft Docs
ms.custom: 
ms.date: 03/02/2016
ms.prod: sql-server-2016
ms.reviewer: 
ms.suite: 
ms.technology:
- analysis-services
ms.tgt_pltfrm: 
ms.topic: language-reference
f1_keywords:
- DATAMEMBER
dev_langs:
- kbMDX
helpviewer_keywords:
- DataMember function
ms.assetid: 65bf21e8-1cb2-4ae8-bfbe-bb4d72589557
caps.latest.revision: 30
author: Minewiskan
ms.author: owend
manager: erikre
ms.translationtype: MT
ms.sourcegitcommit: 1419847dd47435cef775a2c55c0578ff4406cddc
ms.openlocfilehash: b6be9e31f666eafaba1ec7ad346a7e5bb28da9b0
ms.contentlocale: de-de
ms.lasthandoff: 08/02/2017

---
# <a name="datamember-mdx"></a>DataMember (MDX)
[!INCLUDE[tsql-appliesto-ss2008-xxxx-xxxx-xxx_md](../includes/tsql-appliesto-ss2008-xxxx-xxxx-xxx-md.md)]

  Gibt das systemgenerierte Datenelement zurück, das einem Nicht-Blattelement einer Dimension zugeordnet ist.  
  
## <a name="syntax"></a>Syntax  
  
```  
  
Member_Expression.DataMember  
```  
  
## <a name="arguments"></a>Argumente  
 *Member_Expression*  
 Ein gültiger MDX-Ausdruck (Multidimensional Expressions), der ein Element zurückgibt.  
  
## <a name="remarks"></a>Hinweise  
 Diese Funktion nimmt Nichtblattelemente in einer beliebigen Hierarchie und kann verwendet werden, indem Sie die [UPDATE CUBE-Anweisung (MDX)](../mdx/mdx-data-manipulation-update-cube.md) um Daten zu direkt einem Nichtblattelement anstatt auf das Blattelement Nachfolger.  
  
> [!NOTE]  
>  Gibt das angegebene Element zurück, wenn es ein Blattelement ist, oder wenn das Nichtblattelement über keine dazugehörigen Datenelemente verfügt.  
  
## <a name="example"></a>Beispiel  
 Im folgenden Beispiel wird die **DataMember** Funktion in einem berechneten Measure, um die Vertriebsvorgaben für jeden einzelnen Mitarbeiter anzuzeigen:  
  
```  
WITH MEMBER measures.InvidualQuota AS   
([Employee].[Employees].currentmember.datamember, [Measures].[Sales Amount Quota])  
,FORMAT_STRING='Currency'  
SELECT {[Measures].[Sales Amount Quota],[Measures].InvidualQuota} ON COLUMNS,  
[Employee].[Employees].MEMBERS ON ROWS  
FROM [Adventure Works]  
```  
  
## <a name="see-also"></a>Siehe auch  
 [MDX-Funktionsreferenz &#40; MDX &#41;](../mdx/mdx-function-reference-mdx.md)   
 [Schlüsselkonzepte in MDX &#40; Analysis Services &#41;](../analysis-services/multidimensional-models/mdx/key-concepts-in-mdx-analysis-services.md)  
  
  
