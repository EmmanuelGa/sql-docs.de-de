---
title: Standard-Datenquelle | Microsoft Docs
ms.custom: 
ms.date: 01/19/2017
ms.prod: sql-non-specified
ms.reviewer: 
ms.suite: 
ms.technology:
- drivers
ms.tgt_pltfrm: 
ms.topic: article
helpviewer_keywords:
- data sources [ODBC], connection functions
- connecting to data source [ODBC], default data source
- functions [ODBC], data source or driver connections
- data sources [ODBC], default
- default data source [ODBC]
- connecting to data source [ODBC], functions
- connecting to driver [ODBC], default data source
- connecting to driver [ODBC], functions
- connection functions [ODBC]
- ODBC drivers [ODBC], connection functions
ms.assetid: dd473cc6-f051-4aa0-ab14-3dd1b37fe99e
caps.latest.revision: 5
author: MightyPen
ms.author: genemi
manager: jhubbard
ms.translationtype: MT
ms.sourcegitcommit: f7e6274d77a9cdd4de6cbcaef559ca99f77b3608
ms.openlocfilehash: 08c8aab7a9cfcecf18181dacbab6f18aaa59ff64
ms.contentlocale: de-de
ms.lasthandoff: 09/09/2017

---
# <a name="default-data-source"></a>Standard-Datenquelle
Der Treiber kann wählen Sie eine Datenquelle, die Standarddatenquelle in bestimmten Fällen, in denen die Anwendung keine explizit angeben wird, aufgerufen:  
  
-   In einem Aufruf von **SQLConnect** , in dem die *ServerName* Argument ist eine Zeichenfolge der Länge 0 (null), ein null-Zeiger oder DEFAULT.  
  
-   In einem Aufruf von **SQLDriverConnect** , in denen *InConnectionString* gibt an, entweder **DSN**= Standard oder gibt an, mit der **DSN** Schlüsselwort ein die Datenquelle, die nicht in die Systeminformationen enthalten ist.  
  
 Es ist treiberdefinierten, wie die Standarddatenquelle angegeben wird. Dies kann zur Folge haben Verwaltungsaktion und kann, hängt davon ab, der Benutzer.