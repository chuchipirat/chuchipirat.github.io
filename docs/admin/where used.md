---
layout: home
title: Verfolgungsnachweis
permalink: /admin/where_used
nav_exclude: 
parent: System
search_exclude: true
---
# Verfolgungsnachweis

Der Verfolgungsnachweis ermöglicht es, Rezepte, Produkte und Materialien in der Datenbank zu überprüfen. Dies ist wichtig, um festzustellen, ob ein bestimmtes Objekt gelöscht werden darf oder nicht.

![Screen Verfolgungsnachweis](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/admin/_images/where_used.png?raw=true)

### Vorgehensweise

1. **Wähle einen Artikel aus:** Wähle einen Artikel aus der Dropdown-Liste aus. Beachte, dass sowohl Produkte als auch Materialien in der Liste enthalten sind. Oder:
    
2. **Gib die UID eines Rezepts ein:** Falls du die UID eines spezifischen Rezepts kennst, kannst du sie direkt eingeben. Die UID kann beispielsweise in der URL des Rezepts gefunden werden.
    
3. **Starte den Trace:** Sobald du entweder einen Artikel ausgewählt oder die UID eines Rezeptes eingegeben hast, klicke auf die Schaltfläche `Trace Starten`.
    
4. **Ergebnisse anzeigen:** Im Hintergrund wird eine Cloud-Function ausgeführt, um alle relevanten Dokumente zu sammeln. Die Ergebnisse werden dann in Form einer Liste angezeigt.