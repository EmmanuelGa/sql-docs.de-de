---
title: StayInSync-Eigenschaft | Microsoft Docs
ms.prod: sql
ms.prod_service: connectivity
ms.component: ado
ms.technology: connectivity
ms.custom: ''
ms.date: 01/19/2017
ms.reviewer: ''
ms.suite: sql
ms.tgt_pltfrm: ''
ms.topic: conceptual
apitype: COM
f1_keywords:
- Recordset20::StayInSync
- Recordset20::put_StayInSync
- Recordset20::PutStayInSync
- Recordset20::get_StayInSync
- Recordset20::GetStayInSync
helpviewer_keywords:
- StayInSync property
ms.assetid: 502d69b5-dc9a-455d-b115-a03bd39a552b
caps.latest.revision: 11
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: d4e5067036aaaf36c60a134f825012fdc5facf75
ms.sourcegitcommit: 1740f3090b168c0e809611a7aa6fd514075616bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="stayinsync-property"></a>StayInSync-Eigenschaft
Gibt an, in einer hierarchischen [Recordset](../../../ado/reference/ado-api/recordset-object-ado.md) Objekt, gibt an, ob der Verweis auf die zugrunde liegenden untergeordneten Datensätze (d. h. die *Kapitel*) ändert, wenn die übergeordneten Zeile positionieren Änderungen.  
  
## <a name="settings-and-return-values"></a>Einstellungen und Rückgabewerte  
 Legt fest oder gibt einen **booleschen** Wert. Der Standardwert lautet **True**. Wenn **"true"**, im Kapitel über das wird aktualisiert, wenn das übergeordnete Element **Recordset** objektänderungen-Zeilenposition; Wenn **"false"**, weiterhin im Kapitel zum Verweisen auf Daten in der vorherigen Kapitel Obwohl das übergeordnete Element **Recordset** Objekt Zeilenposition geändert hat.  
  
## <a name="remarks"></a>Hinweise  
 Diese Eigenschaft gilt für hierarchische Recordsets, z. B. von unterstützt die [Microsoft-Datenstrukturierungsdiensts für OLE DB-](../../../ado/guide/appendixes/microsoft-data-shaping-service-for-ole-db-ado-service-provider.md), und muss festgelegt werden, für die übergeordnete **Recordset** vor dem untergeordneten Element  **Recordset** abgerufen wird. Diese Eigenschaft wird das Navigieren in hierarchischen Recordsets vereinfacht.  
  
## <a name="applies-to"></a>Gilt für  
 [Recordset-Objekt (ADO)](../../../ado/reference/ado-api/recordset-object-ado.md)  
  
## <a name="see-also"></a>Siehe auch  
 [Beispiel für StayInSync-Eigenschaft (VB)](../../../ado/reference/ado-api/stayinsync-property-example-vb.md)   
 [Microsoft Data strukturiert werden, Dienst für OLE DB (ADO-Dienstanbieter)](../../../ado/guide/appendixes/microsoft-data-shaping-service-for-ole-db-ado-service-provider.md)
