---
title: "\"InfoMessage\"-Ereignis (ADO) | Microsoft Docs"
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
- Connection::InfoMessage
- InfoMessage
helpviewer_keywords:
- InfoMessage event [ADO]
ms.assetid: 468c87dd-e3bc-4084-9941-94d10743d4e9
caps.latest.revision: 11
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 3216c9dfb31fdc7ac27051d409bbb6c658c2b091
ms.sourcegitcommit: 2ddc0bfb3ce2f2b160e3638f1c2c237a898263f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="infomessage-event-ado"></a>"InfoMessage"-Ereignis (ADO)
Die **InfoMessage** Ereignis wird aufgerufen, wenn eine Warnung, während auftritt eine **ConnectionEvent** Vorgang.  
  
## <a name="syntax"></a>Syntax  
  
```  
  
InfoMessage pError, adStatus, pConnection  
```  
  
#### <a name="parameters"></a>Parameter  
 *pError*  
 Ein [Fehler](../../../ado/reference/ado-api/error-object.md) Objekt. Dieser Parameter enthält alle Fehler, die zurückgegeben werden. Wenn mehrere Fehler zurückgegeben werden, aufgelistet werden die **Fehler** Auflistung, um Sie zu finden.  
  
 *adStatus*  
 Ein [EventStatusEnum](../../../ado/reference/ado-api/eventstatusenum.md) Statuswert. Wenn eine Warnung ausgegeben, *AdStatus* festgelegt ist, um **AdStatusOK** und *pError* die Warnung enthält.  
  
 Bevor Sie dieses Ereignis zurückgegeben wird, legen Sie diesen Parameter auf **AdStatusUnwantedEvent** um nachfolgende Benachrichtigungen zu verhindern.  
  
 *pConnection*  
 Ein [Verbindung](../../../ado/reference/ado-api/connection-object-ado.md) Objekt. Die Verbindung, für die die Warnung aufgetreten ist. Warnungen können beispielsweise auftreten, beim Öffnen einer **Verbindung** Objekt oder dem Ausführen einer [Befehl](../../../ado/reference/ado-api/command-object-ado.md) auf eine **Verbindung**.  
  
## <a name="see-also"></a>Siehe auch  
 [ADO-Ereignisse Modell (VC++-Beispiel)](../../../ado/reference/ado-api/ado-events-model-example-vc.md)   
 [ADO-Ereignis-Handler-Zusammenfassung](../../../ado/guide/data/ado-event-handler-summary.md)   
 [Connection-Objekt (ADO)](../../../ado/reference/ado-api/connection-object-ado.md)
