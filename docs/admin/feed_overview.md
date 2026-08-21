---
layout: default
title: Übersicht Feeds
permalink: docs/admin/feeds_overview
nav_exclude: true
parent: System
search_exclude: true
---
# Feed-Einträge Monitor
{: .no_toc }

---

{: .intern-title }
> ☠️ Admin-Bereich ☠️
>
> Diese Seite ist für die Community-Leader\*innen und System-Admins.

Der Feed-Einträge Monitor listet alle generierten Feed-Einträge im System auf. Die Gesamtanzahl wird oberhalb der Tabelle angezeigt. Über das Suchfeld kannst du nach bestimmten Einträgen suchen.

Die Seite hat zwei Tabs: `Übersicht` und `Löschen`.

![Feed Übersicht](/docs/admin/images/feeds.png)
## Übersicht

Die Tabelle zeigt alle Feed-Einträge mit folgenden Spalten:

- **Öffnen:** öffnet die Detailansicht des Eintrags
- **UID:** eindeutige Kennung des Eintrags
- **Typ:** Art des Feed-Eintrags (z.B. donationConfirmed, eventCreated, userCreated)
- **Datum:** Erstellungszeitpunkt
- **Titel:** Kurzbeschreibung der Aktion
- **Sichtbarkeit:** z.B. «basic»
- **User:** wer die Aktion ausgelöst hat

### Detailansicht

Klickst du auf das Öffnen-Symbol, siehst du alle Details zum Eintrag:

- **Feed-Daten:** UID, Typ, Sichtbarkeit, Titel, Text, Erstellt am
- **User:** UID und Name der auslösenden Person
- **Source Object:** Typ, UID und Name des betroffenen Objekts (z.B. Spende, Event, Rezept)

Die angezeigten Informationen variieren je nach Feed-Typ.

Über `Löschen` kannst du den einzelnen Eintrag entfernen, über `Schliessen` die Detailansicht wieder schliessen.

## Löschen (Tab)

Über den Tab `Löschen` kannst du alle Feed-Einträge löschen, die älter als eine bestimmte Anzahl Tage sind.

{: .note }
> Der minimale Zeitraum beträgt 30 Tage. Das System verhindert das Löschen von Einträgen, die jünger als 30 Tage sind.
