---
title: "Voraussetzungen für Tutorials (Berichts-Generator) | Microsoft-Dokumentation"
ms.custom: 
ms.date: 05/30/2017
ms.prod: reporting-services
ms.prod_service: reporting-services-native
ms.service: 
ms.component: reporting-services
ms.reviewer: 
ms.suite: pro-bi
ms.technology: 
ms.tgt_pltfrm: 
ms.topic: get-started-article
applies_to: SQL Server 2016
ms.assetid: 9b8346a6-f4f4-4ad3-bc98-8f2be342ef2d
caps.latest.revision: "11"
author: maggiesMSFT
ms.author: maggies
manager: kfile
ms.workload: On Demand
ms.openlocfilehash: 63dd6f1be616f092e689f5e1ce7ff2ed12e3ece6
ms.sourcegitcommit: 7e117bca721d008ab106bbfede72f649d3634993
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/09/2018
---
# <a name="prerequisites-for-tutorials-report-builder"></a>Voraussetzungen für Lernprogramme (Berichts-Generator)

Die Tutorials zum Berichts-Generator setzen voraus, dass Sie paginierte Berichte aus [!INCLUDE[ssRSCurrent](../includes/ssrscurrent-md.md)] auf einem Berichtsserver oder einer in einen Berichtsserver integrierten SharePoint-Website anzeigen und speichern können. Für Daten werden in allen Tutorials wörtliche Abfragen verwendet, die von einer SQL Server-Instanz verarbeitet werden müssen.  
  
Wenn Sie keinen Zugriff auf einen Berichtsserver, eine Website oder eine Datenquelle haben, können Sie sich mit Berichts-Generator vertraut machen, indem Sie einen Offlinebericht erstellen. Siehe [Tutorial: Create a Quick Chart Report Offline (Report Builder) (Tutorial: Erstellen eines Quick-Diagrammberichts offline (Berichts-Generator))](../reporting-services/report-builder/tutorial-create-a-quick-chart-report-offline-report-builder.md).  

## <a name="requirements"></a>Anforderungen

Für die Ausführung der Lernprogramme zum Berichts-Generator gelten die folgenden Voraussetzungen:  
  
-   Zugriff auf den Berichts-Generator Sie können den Berichts-Generator auf einem [!INCLUDE[ssRSnoversion_md](../includes/ssrsnoversion-md.md)] -Berichtsserver oder einem [!INCLUDE[ssRSnoversion_md](../includes/ssrsnoversion-md.md)] -Berichtsserver im integrierten SharePoint-Modus ausführen. Nur der erste Schritt ist auf den verschiedenen Servern anders, also das Öffnen des Berichts-Generators.  
  
    Wählen Sie auf einem Berichtsserver **Neu** > **Paginierter Bericht**.
  
    Wählen Sie auf einem Berichtsserver im integrierten SharePoint-Modus in der Registerkarte **Dokumente** die Option **Neues Dokument**und wählen Sie aus der Dropdown-Liste **Berichts-Generator-Bericht**. Beispiel: `http://<servername>/sites/mySite/reports`. Der SharePoint-Administrator muss die Funktion "Berichts-Generator-Bericht" für jede Dokumentbibliothek aktivieren.  
  
-   Sie benötigen die URL zu einem [!INCLUDE[ssRSnoversion_md](../includes/ssrsnoversion-md.md)] -Berichtsserver oder einer in einen [!INCLUDE[ssRSnoversion_md](../includes/ssrsnoversion-md.md)] -Berichtsserver integrierten SharePoint-Website. Sie benötigen Berechtigungen zum Speichern und Anzeigen von Berichten, freigegebenen Datenquellen, freigegebenen Datasets, Berichtsteilen und Modellen. Standardmäßig ist die URL für den Berichtsserver `http://<servername>/reportserver`. Standardmäßig ist die URL für eine SharePoint-Website `http://<sitename>` oder `http://<server>/site`.  
  
-   Den Namen einer SQL Server-Instanz und entsprechende Anmeldeinformationen für den schreibgeschützten Zugriff auf eine beliebige Datenbank. In den Datasetabfragen im Tutorial werden zwar Literaldaten verwendet, die Abfrage muss jedoch von einer SQL Server-Instanz verarbeitet werden, um die für ein Berichtsdataset erforderlichen Metadaten zurückzugeben. Die folgende Verbindungszeichenfolge gibt z. B. nur einen Server an: `data source=<servername>`. Sie müssen Lesezugriff auf die Standarddatenbank besitzen, die Ihnen vom Systemadministrator zugewiesen wird, der Ihnen die Berechtigung für den Zugriff auf den Server gewährt. Sie können auch eine Datenbank entsprechend der folgenden Verbindungszeichenfolge angeben: `data source=<servername>;initial catalog=<database>`.  
  
-   Für das [Tutorial: Kartenbericht (Berichts-Generator)](Tutorial:%20Map%20Report%20\(Report%20Builder\).md) muss der Berichtsserver dafür konfiguriert werden, Bing-Karten im Hintergrund zu unterstützen. Weitere Informationen finden Sie unter [Planen der Unterstützung für Kartenberichte](http://msdn.microsoft.com/en-us/5ddc97a7-7ee5-475d-bc49-3b814dce7e19).   

-   Das [Tutorial: Erstellen von Drillthrough- und Hauptberichten (Berichts-Generator)](Tutorial:%20Creating%20Drillthrough%20and%20Main%20Reports%20\(Report%20Builder\).md) erfordert Zugriff auf den Contoso-Umsatz-Cube. Weitere Informationen finden Sie im Tutorial. 
  
Der Berichtsserveradministrator muss Ihnen die erforderlichen Berechtigungen für den Berichtsserver erteilen und die Orte für die [!INCLUDE[ssRSnoversion_md](../includes/ssrsnoversion-md.md)] -Ordner sowie die Standardoptionen für den Berichts-Generator konfigurieren. Weitere Informationen finden Sie unter [Installieren und Deinstallieren des Berichts-Generators](http://msdn.microsoft.com/library/2c9a5814-17bf-4947-8fb3-6269e7caa416).  

## <a name="next-steps"></a>Nächste Schritte

[Tutorials (Berichts-Generator)](../reporting-services/report-builder-tutorials.md)  

Haben Sie dazu Fragen? [Stellen Sie eine Frage im Reporting Services-Forum](http://go.microsoft.com/fwlink/?LinkId=620231)
