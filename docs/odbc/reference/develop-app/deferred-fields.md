---
title: "Verzögerte Felder | Microsoft Docs"
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
- descriptors [ODBC], deferred fields
- deferred fields [ODBC]
ms.assetid: 5abeb9cc-4070-4f43-a80d-ad6a2004e5f3
caps.latest.revision: 5
author: MightyPen
ms.author: genemi
manager: jhubbard
ms.translationtype: MT
ms.sourcegitcommit: f7e6274d77a9cdd4de6cbcaef559ca99f77b3608
ms.openlocfilehash: 38967637f505191a5ff353c13b4ebfbbe08e615a
ms.contentlocale: de-de
ms.lasthandoff: 09/09/2017

---
# <a name="deferred-fields"></a>Zurückgestellten Felder
Die Werte der *verzögert Felder* werden nicht verwendet werden, wenn sie festgelegt werden, aber der Treiber die Adressen mit den Variablen für eine verzögerte wirksam speichert. Für eine anwendungsparameterdeskriptor, verwendet der Treiber den Inhalt der Variablen zum Zeitpunkt des Aufrufs von **SQLExecDirect** oder **SQLExecute**. Für eine Anwendung Zeilendeskriptor verwendet der Treiber den Inhalt der Variablen zum Zeitpunkt des Abrufs.  
  
 Es folgen zurückgestellten Felder:  
  
-   Die Felder SQL_DESC_DATA_PTR und SQL_DESC_INDICATOR_PTR anwendungsparameterdeskriptor-Datensatz.  
  
-   Das Feld SQL_DESC_OCTET_LENGTH_PTR von einer Anwendung anwendungsparameterdeskriptor-Datensatz.  
  
-   Im Fall einer Einfügung mehrerer Zeilen abrufen die SQL_DESC_ARRAY_STATUS_PTR und SQL_DESC_ROWS_PROCESSED_PTR Felder eines Deskriptor-Headers.  
  
 Wenn ein Deskriptor, der belegt wurde, haben die verzögerte Felder der einzelnen anwendungsparameterdeskriptor-Datensatz zunächst einen null-Wert. Die Bedeutung des null-Werts lautet wie folgt:  
  
-   Wenn SQL_DESC_ARRAY_STATUS_PTR einen null-Wert aufweist, schlägt ein Abrufs mehrzeiligen diese Komponente Diagnoseinformationen pro Zeile zurückgeben.  
  
-   Wenn SQL_DESC_DATA_PTR einen null-Wert aufweist, wird der Datensatz aufgehoben.  
  
-   Wenn Feld SQL_DESC_OCTET_LENGTH_PTR ein ARD einen null-Wert aufweist, gibt der Treiber Längeninformationen für diese Spalte keinen zurück.  
  
-   Wenn Feld SQL_DESC_OCTET_LENGTH_PTR ein APD einen null-Wert hat, und der Parameter eine Zeichenfolge ist, wird vom Treiber angenommen, dass Null-terminierte Zeichenfolge ist. Für dynamische Output-Parameter verhindert, dass ein null-Wert in diesem Feld den Treiber Längeninformationen zurückgeben. (Wenn das SQL_DESC_TYPE-Feld einen Zeichenfolge Parameter nicht angegeben ist, wird das Feld SQL_DESC_OCTET_LENGTH_PTR ignoriert.)  
  
 Die Anwendung muss nicht freigeben oder verwerfen Variablen für verzögerte Felder zwischen dem Zeitpunkt, der sie die Felder zuordnet und die Uhrzeit, die der Treiber liest oder schreibt sie, verwendet wird.