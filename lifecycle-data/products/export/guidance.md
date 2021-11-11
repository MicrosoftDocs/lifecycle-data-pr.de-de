---
title: Informationen zum Lebenszyklus-Datenexport
description: Informationen zum Export von Produktlebenszyklusinformationen
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546798"
---
# <a name="lifecycle-data-export-guidance"></a>Informationen zum Lebenszyklus-Datenexport
In diesem Dokument wird die Verwendung der Produktexportdatei beschrieben.

## <a name="query-information"></a>Abfrageninformationen
Das Excel-Dokument enthält Felder zur Identifizierung der in der Produkttabelle aufgefüllten Daten.

### <a name="end-of-support"></a>End Of Support
Der Wert für „end of support“ filtert Produkte entweder nach dem Datum des Supportendes oder dem Versionsende eines Produkts.

Mögliche Werte: „All“ (kein Filter angewendet), „Year“ und „Range“.

### <a name="family"></a>Family
Der Wert „Family“ filtert Produkte nach der übergeordneten Ebene innerhalb der Hierarchie, die als „Familie“ bezeichnet wird.

Mögliche Werte: „All“ (kein Filter angewendet), „Family Name“

### <a name="group"></a>Gruppe
Der Gruppenwert filtert Produkte innerhalb der übergeordneten Ebene (Familie) nach einer bestimmten Gruppe.

Mögliche Werte: „All“ (kein Filter angewendet), Gruppenname

## <a name="table-columns"></a>Tabellenspalten
Die Produkttabelle besteht aus Spalten, die das Produkt, die Editionen, die Versionen und die entsprechenden Supportdaten definieren.

> [!NOTE]
> Sie enthält eine Zeile für jede Kombination aus Produkt, Edition und Version.

### <a name="product"></a>Produkt
Produktname

### <a name="edition"></a>Edition
Die Spalte „edition“ wird ausgefüllt, wenn das Produkt Editionen enthält. Wenn keine Produktedition vorhanden ist, ist dieses Feld leer.

### <a name="release"></a>Freigabe
Die Spalte „release“ wird ausgefüllt, wenn das Produkt mehrere Versionen enthält.
Wenn das Produkt nur eine Version aufweist, ist dieses Feld leer.

### <a name="support-policy"></a>Support Policy
In diesem Feld wird definiert, welcher Supportrichtlinie das Produkt folgt.

Mögliche Werte: [Fixed](/lifecycle/policies/fixed), [Modern](/lifecycle/policies/modern), Component

### <a name="start-date"></a>Anfangstermin
Datum, an dem der Support für das Produkt anfing.

### <a name="mainstream-date"></a>Mainstream Date
Lautet die Supportrichtlinie **Fixed** oder **Component**, ist dies das Ablaufdatum des allgemeinen Supports des Produkts.
  
Lautet die Supportrichtlinie **Modern**, ist dieses Feld leer.

### <a name="extended-end-date"></a>Extended End Date
Bei der Supportrichtlinie **Fixed** oder **Component**, ist dies das Datum des verlängerten Ablaufdatums des Produkts.

Lautet die Supportrichtlinie **Modern**, ist dieses Feld leer.

### <a name="retirement-date"></a>Retirement Date
Lautet die Supportrichtlinie **Fixed** oder **Component**, ist dieses Feld leer.

Lautet die Supportrichtlinie **Modern**, ist dies das Deaktivierungsdatum des Produkts.

### <a name="release-start-date"></a>Release Start Date
Datum, an dem der Support für diese Version anfing. Wenn das Produkt nur eine Version aufweist, ist dieses Feld leer.
 
### <a name="release-end-date"></a>Release End Date
Datum, an dem der Support für die Version beendet wurde.
Wenn das Produkt nur eine Version aufweist, ist dieses Feld leer.

### <a name="docs-url"></a>Docs Url
URL zur weiterführenden Dokumentation.
