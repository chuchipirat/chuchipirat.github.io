---
layout: default
title: Mengenberechnung
nav_exclude: false
has_children: false
nav_order: 3
parent: Anlass
---
# Mengenberechnung
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

Die Mengenberechnung ist das Herzstück der Portionenplanung im chuchipirat. Hier definierst du, wie sich deine Gruppe zusammensetzt — welche Essensvorlieben (Fleisch, Vegetarisch, Vegan usw.) und Unverträglichkeiten (Laktose, Gluten usw.) es gibt und wie viele Personen zu welcher Kombination gehören.

## Wie funktioniert das?

Der Ablauf ist folgender:

1. **Hier:** Du definierst die Gruppen und trägst die Anzahl Portionen pro Kombination ein.
2. **Im Menüplan:** Wenn du ein Rezept einem Menü hinzufügst, wählst du aus, für welche Gruppen und Unverträglichkeiten das Rezept bestimmt ist. Anhand dieser Auswahl berechnet der chuchipirat die Gesamtportionen und skaliert das Rezept entsprechend.
3. **Bei Änderungen:** Ändert sich die Gruppengrösse (z.B. weil kurzfristig mehr Vegetarier\*innen dabei sind), passt du hier die Zahlen an — und alle verknüpften Rezepte werden automatisch neu skaliert.

{: .highlight }
Der grosse Vorteil gegenüber fixen Portionen: Du änderst die Gruppengrösse an **einem** Ort, und alle Rezepte passen sich automatisch an.

## Beispiel

![Beispiel Mengenberechnung](/docs/event/images/groupconfiguration_change_settings.png)

In diesem Beispiel gibt es zwei Essensgruppen (Fleisch und Vegetarisch) und drei Unverträglichkeits-Zeilen. Von den 14 Fleischesser\*innen haben 2 eine Laktoseintoleranz. Dazu kommen 6 Vegetarier\*innen, davon ebenfalls 2 mit Laktoseintoleranz. Total wird für 20 Personen geplant.

{: .note }
Wenn dir das mit den Gruppen zu kompliziert erscheint, trage einfach die Gesamtanzahl Portionen im ersten Feld ein und lass die anderen leer. Du kannst auch im Menüplan die Option «Fixe Portionen» pro Rezept verwenden.

## Portionen anpassen

Ändert sich die Gruppenzusammensetzung, trägst du die neuen Zahlen ein. Sobald der chuchipirat eine Änderung erkennt, erscheinen zwei Buttons:

- `Speichern und Portionen neu berechnen` — übernimmt die neuen Werte und berechnet alle geplanten Rezepte neu
- `Änderungen verwerfen` — lädt die zuletzt gespeicherten Werte

## Gruppen und Unverträglichkeiten verwalten

### Hinzufügen

Klicke auf `+` in den Spaltenüberschriften (für eine neue Essensgruppe) oder auf `+ Unverträglichkeit` (für eine neue Zeile). Gib der Gruppe den gewünschten Namen.

### Umbenennen

Klicke auf die drei vertikalen Punkte ⋮ neben der Gruppe und wähle «Umbenennen». Die Änderung wird erst nach dem Speichern aktiv.

{: .important }
Bereits geplante Rezepte bleiben mit der Gruppe verknüpft — auch wenn der Name nun etwas anderes aussagt. Benennst du z.B. «Fleisch» in «Vegan» um, sind die Fleischrezepte weiterhin mit dieser Gruppe verknüpft.

### Löschen

Klicke auf die drei vertikalen Punkte ⋮ und wähle «Löschen». Die Änderung wird erst nach dem Speichern aktiv.

{: .warning }
Löschst du eine Gruppe, wird auch die Verknüpfung der geplanten Rezepte zu dieser Gruppe gelöscht. Es kann sein, dass Rezepte danach nur noch für wenige Teilgruppen oder gar niemanden geplant sind.
