---
title: Bearbeiten vorhandener Einträge | Microsoft Docs
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
helpviewer_keywords:
- editing data [ADO], existing records
ms.assetid: 17ce1263-5897-452a-9ea5-c7f96b33df65
caps.latest.revision: 10
author: MightyPen
ms.author: genemi
manager: craigg
ms.openlocfilehash: f6caa67868172118f7e70b1781b7fbb08ec22641
ms.sourcegitcommit: 2ddc0bfb3ce2f2b160e3638f1c2c237a898263f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
---
# <a name="editing-existing-records"></a>Bearbeiten vorhandener Einträge
Um vorhandene Datensätze zu bearbeiten, verschieben, auf die Zeile, die Sie verwenden möchten, bearbeiten und ändern Sie die **Wert** Eigenschaft der Felder, die Sie ändern möchten. Weitere Informationen zu den **Feld** des Objekts **Wert** Eigenschaft finden Sie unter [Untersuchen von Daten](../../../ado/guide/data/examining-data.md). Verwenden Sie abhängig vom Cursortyp **Update** oder **UpdateBatch** zum Senden von Änderungen an der Datenquelle. Weitere Informationen finden Sie unter [wird aktualisiert und Beibehalten von Daten](../../../ado/guide/data/updating-and-persisting-data.md).  
  
 Es ist in der Regel effizienter, eine gespeicherte Prozedur mit einer Command-Objekt zu verwenden, um Updates, die auch ausgeführt werden als andere Vorgänge ausführen, da eine gespeicherte Prozedur nicht die Erstellung eines Cursors erfordert. Weitere Informationen zu Cursorn finden Sie unter [Grundlegendes zu Cursorn und Sperren](../../../ado/guide/data/understanding-cursors-and-locks.md).
