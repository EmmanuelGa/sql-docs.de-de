---
title: DISCOVER_CONNECTIONS-Rowset | Microsoft Docs
ms.date: 05/03/2018
ms.prod: sql
ms.technology: analysis-services
ms.component: schema-rowsets
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
ms.openlocfilehash: de0346d7412f55e597db4b7b44cd533114a297a5
ms.sourcegitcommit: f1caaa156db2b16e817e0a3884394e7b30fb642f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="discoverconnections-rowset"></a>DISCOVER_CONNECTIONS-Rowset
[!INCLUDE[ssas-appliesto-sqlas](../../../includes/ssas-appliesto-sqlas.md)]
  Stellt Informationen zur Ressourcenverwendung und Aktivität der zurzeit geöffneten Verbindungen auf dem Server bereit.  
  
 **Gilt für:** tabellarische und mehrdimensionale Modelle  
  
## <a name="rowset-columns"></a>Rowsetspalten  
 Das **DISCOVER_CONNECTIONS** -Rowset enthält die folgenden Spalten.  
  
|Spaltenname|Typindikator|Einschränkungen|Description|  
|-----------------|--------------------|------------------|-----------------|  
|**CONNECTION_ID**|**DBTYPE_I4**|ja|Eine eindeutige Zahl, die die Verbindung identifiziert.|  
|**CONNECTION_USER_NAME**|**DBTYPE_WSTR**|ja|Der Name des Benutzers dieser Verbindung.|  
|**CONNECTION_IMPERSONATED_USER_NAME**|**DBTYPE_WSTR**|ja|Zur künftigen Verwendung reserviert. Analysis Services geben immer NULL für den Wert von CONNECTION_IMPERSONATED_USER_NAME zurück.|  
|**CONNECTION_HOST_NAME**|**DBTYPE_WSTR**|ja|Der Name des Computers, der die Verbindung initiiert hat.|  
|**CONNECTION_HOST_APPLICATION**|**DBTYPE_WSTR**||Der Name der Anwendung, die die Verbindung initiiert hat.|  
|**CONNECTION_START_TIME**|**DBTYPE_DBTIMESTAMP**||UTC-Datum und -Zeit des Servers, zu denen die Verbindung initiiert wurde.|  
|**CONNECTION_ELAPSED_TIME_MS**|**DBTYPE_I8**|ja|Seit dem Start der Verbindung verstrichene Zeit in Millisekunden.|  
|**CONNECTION_LAST_COMMAND_START_TIME**|**DBTYPE_DBTIMESTAMP**||UTC-Datum und -Zeit des Servers, zu denen der letzte Befehl seine Ausführung initiiert hat.|  
|**CONNECTION_LAST_COMMAND_END_TIME**|**DBTYPE_DBTIMESTAMP**||UTC-Datum und -Zeit des Servers, zu denen der letzte Befehl seine Ausführung beendet hat.|  
|**CONNECTION_LAST_COMMAND_ELAPSED_TIME_MS**|**DBTYPE_I8**|ja|Die seit dem Ende der Ausführung des letzten Befehls verstrichene Zeit in Millisekunden.|  
|**CONNECTION_IDLE_TIME_MS**|**DBTYPE_I8**|ja|Die Leerlaufzeit in Millisekunden seit dem Start der Verbindung.|  
|**CONNECTION_BYTES_SENT**|**DBTYPE_I8**||Die akkumulierte Zahl der seit dem Start der Verbindung von der Verbindung gesendeten Bytes.|  
|**CONNECTION_DATA_BYTES_SENT**|**DBTYPE_I8**||Die akkumulierte Zahl der seit dem Start der Verbindung von der Verbindung gesendeten Datenbytes.<br /><br /> Daten werden innerhalb der Verbindung in komprimierter Form ausgetauscht. Dieser Wert gibt die Menge der gesendeten extrahierten Daten wieder.|  
|**CONNECTION_BYTES_RECEIVED**|**DBTYPE_I8**||Die akkumulierte Zahl der seit dem Start der Verbindung von der Verbindung empfangenen Bytes.|  
|**CONNECTION_DATA_BYTES_RECEIVED**|**DBTYPE_I8**||Die akkumulierte Zahl der seit dem Start der Verbindung von der Verbindung empfangenen Datenbytes.<br /><br /> Daten werden innerhalb der Verbindung in komprimierter Form ausgetauscht. Dieser Wert gibt die Menge der empfangenen extrahierten Daten wieder.|  
  
 Dieses Schemarowset ist nicht sortiert.  
  
## <a name="using-adomdnet-to-return-the-rowset"></a>Verwenden von ADOMD.NET zum Zurückgeben des Rowsets  
 Wenn Sie Metadaten mithilfe von ADOMD.NET und des Schemarowsets abrufen, können Sie entweder die GUID verwenden oder eine Referenz für ein Schemarowsetobjekt in der GetSchemaDataSet-Methode herstellen. Weitere Informationen finden Sie unter [Working with Schema Rowsets in ADOMD.NET](../../../analysis-services/multidimensional-models-adomd-net-client/retrieving-metadata-working-with-schema-rowsets.md).  
  
 Die folgende Tabelle enthält die GUID und die Zeichenfolgenwerte, die dieses Rowset identifizieren.  
  
|Argument|Wert|  
|--------------|-----------|  
|GUID|a07ccd25-8148-11d0-87bb-00c04fc33942|  
|ADOMDNAME|Verbindungen|  
  
## <a name="see-also"></a>Siehe auch  
 [XML for Analysis-Schemarowsets](../../../analysis-services/schema-rowsets/xml/xml-for-analysis-schema-rowsets.md)  
  
  
