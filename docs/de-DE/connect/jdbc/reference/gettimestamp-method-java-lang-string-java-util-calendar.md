---
title: GetTimestamp-Methode (java.lang.String, java.util.Calendar) | Microsoft Docs
ms.custom: ''
ms.date: 01/19/2017
ms.prod: sql
ms.prod_service: drivers
ms.service: ''
ms.component: jdbc
ms.reviewer: ''
ms.suite: sql
ms.technology:
- drivers
ms.tgt_pltfrm: ''
ms.topic: conceptual
apiname:
- SQLServerCallableStatement.getTimestamp (java.lang.String,java.util.Calendar)
apilocation:
- sqljdbc.jar
apitype: Assembly
ms.assetid: 770668d9-2e52-4ff0-be2f-ebf78fd41644
caps.latest.revision: 10
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: 310374294313d7eca6ea3aa8e821254e07b67d27
ms.sourcegitcommit: 2ddc0bfb3ce2f2b160e3638f1c2c237a898263f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="gettimestamp-method-javalangstring-javautilcalendar"></a>getTimestamp-Methode (java.lang.String, java.util.Calendar)
[!INCLUDE[Driver_JDBC_Download](../../../includes/driver_jdbc_download.md)]

  Ruft den Wert des angegebenen Parameters als java.sql.Timestamp-Objekt in der Programmiersprache Java ab, Berücksichtigung des Parameternamens, unter Verwendung eines Kalenders-Objekts ab.  
  
## <a name="syntax"></a>Syntax  
  
```  
  
public java.sql.Timestamp getTimestamp(java.lang.String name,  
                                       java.util.Calendar cal)  
```  
  
#### <a name="parameters"></a>Parameter  
 *name*  
  
 Ein **Zeichenfolge** , die den Namen des Parameters enthält.  
  
 *CAL*  
  
 Ein Kalenderobjekt.  
  
## <a name="return-value"></a>Rückgabewert  
 Eine Timestamp-Objekt.  
  
## <a name="exceptions"></a>Ausnahmen  
 [SQLServerException](../../../connect/jdbc/reference/sqlserverexception-class.md)  
  
## <a name="remarks"></a>Hinweise  
 Diese GetTimestamp-Methode wird von der GetTimestamp-Methode in der java.sql.CallableStatement-Schnittstelle angegeben.  
  
 Diese Methode gibt nur Werte aus [!INCLUDE[ssNoVersion](../../../includes/ssnoversion_md.md)] **"DateTime"** und **Smalldatetime** Spalten.  
  
## <a name="see-also"></a>Siehe auch  
 [GetTimestamp-Methode &#40;SQLServerCallableStatement&#41;](../../../connect/jdbc/reference/gettimestamp-method-sqlservercallablestatement.md)   
 [SQLServerCallableStatement-Elemente](../../../connect/jdbc/reference/sqlservercallablestatement-members.md)   
 [SQLServerCallableStatement-Klasse](../../../connect/jdbc/reference/sqlservercallablestatement-class.md)  
  
  
