---
title: GetString-Methode (Int) | Microsoft Docs
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
- SQLServerCallableStatement.getString (int)
apilocation:
- sqljdbc.jar
apitype: Assembly
ms.assetid: f3fce8bf-8d6e-476f-aa6d-992daa79b899
caps.latest.revision: 10
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: bc00f8c9057f0b4222603ccb281251d9b240aab8
ms.sourcegitcommit: 2ddc0bfb3ce2f2b160e3638f1c2c237a898263f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="getstring-method-int"></a>getString-Methode (int)
[!INCLUDE[Driver_JDBC_Download](../../../includes/driver_jdbc_download.md)]

  Ruft den Wert des angegebenen Parameters als eine **Zeichenfolge** in der Berücksichtigung des parameterindexes Programmiersprache Java ab.  
  
## <a name="syntax"></a>Syntax  
  
```  
  
public java.lang.String getString(int index)  
```  
  
#### <a name="parameters"></a>Parameter  
 *index*  
  
 Ein **Int** , der die Indexnummer des Parameters angibt.  
  
## <a name="return-value"></a>Rückgabewert  
 Ein **Zeichenfolge** Wert.  
  
## <a name="exceptions"></a>Ausnahmen  
 [SQLServerException](../../../connect/jdbc/reference/sqlserverexception-class.md)  
  
## <a name="remarks"></a>Hinweise  
 Diese GetString-Methode wird von der GetString-Methode in der java.sql.CallableStatement-Schnittstelle angegeben.  
  
 Alle Spalten in [!INCLUDE[ssNoVersion](../../../includes/ssnoversion_md.md)] als Zeichenfolge zurückgegeben werden kann. Es können also eine Zeichenfolgendarstellung aller zahlen- und zeichenfolgenbasierten Typen und eine hexadezimale Zeichenfolgendarstellung binärer Spalten wie "binary", "varbinary", "varbinary(max)", "image", "timestamp" oder "uniqueidentifier" zurückgegeben werden.  
  
 Speicherort sicherheitskritische Typen wie z. B. Money, Smallmoney, Datetime, Smalldatetime, Float, real, decimal und numeric werden für den zugrunde liegenden Wert des Typs das kanonische ToString()-Format zurück.  
  
 Benutzerdefinierte Typen werden als hexadezimale Zeichenfolgenwerte zurückgegeben.  
  
## <a name="see-also"></a>Siehe auch  
 [GetString-Methode &#40;SQLServerCallableStatement&#41;](../../../connect/jdbc/reference/getstring-method-sqlservercallablestatement.md)   
 [SQLServerCallableStatement-Elemente](../../../connect/jdbc/reference/sqlservercallablestatement-members.md)   
 [SQLServerCallableStatement-Klasse](../../../connect/jdbc/reference/sqlservercallablestatement-class.md)  
  
  
