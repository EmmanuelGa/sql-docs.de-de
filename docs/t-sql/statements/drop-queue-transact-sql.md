---
title: DROP QUEUE (Transact-SQL) | Microsoft Docs
ms.custom: 
ms.date: 03/06/2017
ms.prod: sql-non-specified
ms.reviewer: 
ms.suite: 
ms.technology:
- database-engine
ms.tgt_pltfrm: 
ms.topic: language-reference
f1_keywords:
- DROP QUEUE
- DROP_QUEUE_TSQL
dev_langs:
- TSQL
helpviewer_keywords:
- dropping queues
- queues [Service Broker], removing
- deleting queues
- DROP QUEUE statement
- removing queues
ms.assetid: fd866520-ca00-477d-b2e9-0110e9610ed4
caps.latest.revision: 33
author: JennieHubbard
ms.author: jhubbard
manager: jhubbard
ms.translationtype: MT
ms.sourcegitcommit: 876522142756bca05416a1afff3cf10467f4c7f1
ms.openlocfilehash: 51920e14a3a24f9bfb48f11c07414812da1694b9
ms.contentlocale: de-de
ms.lasthandoff: 09/01/2017

---
# <a name="drop-queue-transact-sql"></a>DROP QUEUE (Transact-SQL)
[!INCLUDE[tsql-appliesto-ss2008-xxxx-xxxx-xxx_md](../../includes/tsql-appliesto-ss2008-xxxx-xxxx-xxx-md.md)]

  Löscht eine vorhandene Warteschlange.  
  
 ![Themenlinksymbol](../../database-engine/configure-windows/media/topic-link.gif "Topic link icon") [Transact-SQL Syntax Conventions (Transact-SQL-Syntaxkonventionen)](../../t-sql/language-elements/transact-sql-syntax-conventions-transact-sql.md)  
  
## <a name="syntax"></a>Syntax  
  
```  
  
DROP QUEUE <object>  
[ ; ]  
  
<object> ::=  
{  
    [ database_name . [ schema_name ] . | schema_name . ]  
        queue_name  
}  
```  
  
## <a name="arguments"></a>Argumente  
 *database_name*  
 Der Name der Datenbank, die die zu löschende Warteschlange enthält. Wenn kein *Database_name* angegeben ist, wird der Standardwert ist der aktuellen Datenbank.  
  
 *Schema_name (Objekt)*  
 Der Name des Schemas, das die zu löschende Warteschlange besitzt. Wenn kein *Schema_name* angegeben ist, wird der Standardwert ist das Standardschema für den aktuellen Benutzer.  
  
 *Warteschlangenname*  
 Der Name der zu löschenden Warteschlange.  
  
## <a name="remarks"></a>Hinweise  
 Sie können eine Warteschlange nicht löschen, wenn Dienste auf sie verweisen.  
  
## <a name="permissions"></a>Berechtigungen  
 Berechtigung zum Löschen einer Warteschlange wird standardmäßig beim Besitzer der Warteschlange, bei Mitgliedern der der **Db_ddladmin** oder **Db_owner** festen Datenbankrollen und Mitglieder der **Sysadmin** behoben Serverrolle.  
  
## <a name="examples"></a>Beispiele  
 Das folgende Beispiel löscht die **ExpenseQueue** Warteschlange aus der aktuellen Datenbank.  
  
```  
DROP QUEUE ExpenseQueue ;  
  
```  
  
## <a name="see-also"></a>Siehe auch  
 [CREATE QUEUE &#40;Transact-SQL&#41;](../../t-sql/statements/create-queue-transact-sql.md)   
 [ALTER QUEUE &#40; Transact-SQL &#41;](../../t-sql/statements/alter-queue-transact-sql.md)   
 [EVENTDATA &#40;Transact-SQL&#41;](../../t-sql/functions/eventdata-transact-sql.md)  
  
  