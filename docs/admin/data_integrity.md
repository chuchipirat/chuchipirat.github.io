---
layout: default
title: Datenintegrität
nav_exclude: true
parent: System
search_exclude: true
---
# Datenintegrität
{: .no_toc }

<details markdown="block">
  <summary>
    Inhalt
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

---

{: .intern-title }
> ☠️ Admin-Bereich ☠️
>
> Diese Seite ist für die System-Admins.

Die Datenintegrität prüft die Konsistenz der Daten im chuchipirat. Über den Button `Alle Integritätstests starten` werden alle Prüfungen auf einmal ausgeführt. Alternativ kannst du einzelne Abschnitte aufklappen und gezielt prüfen.

Jeder Abschnitt zeigt nach der Prüfung ein farbiges Badge:
- **Grün** — keine Auffälligkeiten gefunden
- **Orange** — Einträge gefunden, die überprüft werden sollten

Bei den gefundenen Einträgen kannst du über die Icons direkt zum Bearbeiten oder Löschen des jeweiligen Items navigieren.

![Datenintegrität](/docs/admin/images/data_integrity.png)
## Prüfungen

### Verwaiste Rezepte

Findet Rezepte, deren Produkte nicht mehr existieren. Das kann passieren, wenn ein Produkt gelöscht wurde, das noch in einem Rezept verwendet wird.

### Verwaiste Event-Küche

Findet Event-Küchen-Einträge, die keinem bestehenden Event mehr zugeordnet sind.

### Events ohne Zeitschedule

Findet Events, denen keine Zeitschedule zugeordnet ist.

### Unbenutzte Produkte

Listet Produkte auf, die in keinem Rezept, keiner Menüplanung und keiner Einheitenumrechnung referenziert werden. Diese Produkte können potenziell bereinigt werden.

### Unbenutzte Materialien

Listet Materialien auf, die in keinem Rezept und keiner Menüplanung referenziert werden.

### Rezepte ohne Event

Zeigt öffentliche Rezepte, die in keinem Event, Anlass oder Menü verwendet werden.
