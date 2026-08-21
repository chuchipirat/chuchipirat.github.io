---
layout: default
title: Menüplan
nav_exclude: false
has_children: false
nav_order: 3
parent: Anlass
---
# Menüplan
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

Der Menüplan ist das Herzstück deines Anlasses. Hier legst du fest, wann du welche Rezepte kochen möchtest, und kannst [Notizen](#notizen), [Produkte und Materialien](#produkte-und-materialien) für einzelne Menüs hinterlegen.

## Struktur

Der Menüplan ist als Tabelle aufgebaut:

- **Spalten = Tage** — für jeden Tag deines Anlasses gibt es eine Spalte. Die Anpassung der Tage erfolgt in den [Infos zum Anlass]({% link docs/event/event_settings.md %}).
{::comment}[[event_settings]]{:/comment}
- **Zeilen = Mahlzeiten** — standardmässig «Zmorgen», «Zmittag» und «Znacht». Du kannst Mahlzeiten [hinzufügen](#mahlzeit-hinzufügen), [umbenennen](#mahlzeit-umbenennen), [verschieben](#mahlzeit-verschieben) oder [löschen](#mahlzeit-löschen).
- **Karten = Menüs** — ein Menü ist eine Sammlung von Rezepten, Produkten und Materialien, die an einem Tag zu einer bestimmten Mahlzeit geplant werden. Eine Mahlzeit kann mehrere Menüs haben (z.B. ein Fleisch- und ein Vegetarisch-Menü).

## Schalter

Oberhalb des Menüplans findest du zwei Schalter:

- **Details anzeigen** — zeigt bei jedem Rezept die geplanten Portionen und die verknüpften Gruppen an
- **Drag & Drop aktivieren** — ermöglicht das Verschieben von Menüs und Mahlzeiten per Drag and Drop

## Rezepte

### Rezept hinzufügen

Klicke auf `Rezept Hinzufügen +` in der gewünschten Menükarte. Es öffnet sich die Rezeptübersicht mit allen öffentlichen Rezepten, deinen privaten Rezepten und den Varianten dieses Anlasses. Du kannst die [Suche und Filter]({% link docs/recipe/recipes_overview.md %}#suche) nutzen, um das passende Rezept zu finden.
{::comment}[[recipes_overview]]{:/comment}

Als Nächstes wählst du, in welchen Menüs das Rezept eingeplant werden soll. Du kannst das Rezept gleich für mehrere Tage/Mahlzeiten planen.

![Dialog Menüauswahl](/docs/event/images/menueplan_choose_menue.png)

Zum Schluss gibst du an, für wie viele Portionen du planst. Du hast zwei Möglichkeiten:

#### Variable Portionen (über Mengenberechnung)

Verknüpfe das Rezept mit einer oder mehreren Gruppen aus der [Mengenberechnung]({% link docs/event/groupconfiguration.md %}). Wähle in der oberen Buttonreihe die Ernährungsgruppe (z.B. «Fleisch» oder «Vegetarisch») und aktiviere die Checkboxen für die Unverträglichkeiten. Rechts siehst du die Portionen pro Auswahl. Optional kannst du einen **Faktor** hinterlegen (z.B. 0.5, wenn du zwei Saucen machst, oder 1.2 nach einem Sportblock).
{::comment}[[groupconfiguration]]{:/comment}

![Dialog Portionen setzen](/docs/event/images/menueplan_set_portions.png)

{: .highlight }
Der Vorteil: Ändert sich die Gruppengrösse in der [Mengenberechnung]({% link docs/event/groupconfiguration.md %}), werden alle verknüpften Rezepte automatisch angepasst.

#### Fixe Portionen

Wähle in der oberen Buttonreihe `Fixe Portionen` und gib die gewünschte Anzahl ein. Diese bleibt unverändert, auch wenn die Mengenberechnung angepasst wird.

Klicke auf `Hinzufügen`, um das Rezept einzuplanen.

### Portionen ändern

Klicke in der Menükarte auf die drei Punkte ⋮ und wähle `Menü bearbeiten`. Klicke auf das Stift-Symbol neben dem Rezept, um die Portionen anzupassen.

![Menü bearbeiten](/docs/event/images/menueplan_edit_menue.png)

### Rezept verschieben

Bei aktiviertem «Drag & Drop» kannst du ein Rezept per Drag and Drop in ein anderes Menü ziehen.

### Rezept aus dem Menüplan entfernen

Klicke auf die drei Punkte ⋮ → `Menü bearbeiten` und dann auf das Mülleimer-Symbol beim entsprechenden Rezept.

{: .highlight }
Wird ein [Rezept gänzlich gelöscht]({% link docs/recipe/recipe_structure.md %}#rezept-löschen) (nicht nur aus dem Menüplan entfernt), wird in allen betroffenen Menüs ein Hinweis hinterlassen.

![Gelöschtes Rezept](/docs/event/images/menueplan_deleted_recipe.png)

## Menü

Ein Menü sammelt alle Rezepte, Produkte und Materialien für eine Mahlzeit. Du kannst dem Menü einen Namen geben — dieser erscheint in den diversen Dialogen und erleichtert die Orientierung. Rezepte, Produkte und Materialien werden direkt in der Menükarte angezeigt.

### Neues Menü erstellen

Klicke in einer Mahlzeit, die noch kein Menü hat, auf `Neues Menü`. Falls alle Mahlzeiten bereits ein Menü haben, verschiebe eines temporär an einen anderen Ort, erstelle das neue Menü an der frei gewordenen Stelle und verschiebe das andere zurück.

![Neues Menü erstellen](/docs/event/images/menuplan_create_new_menue.png)

### Menü verschieben

Bei aktiviertem «Drag & Drop» kannst du ein Menü per Drag and Drop an eine andere Stelle ziehen.

![Menü verschieben](/docs/event/images/menueplan_move_menue.gif)

### Menü löschen

Klicke in der Menükarte auf die drei Punkte ⋮ und wähle `Menü löschen`.

{: .warning }
Gelöschte Menüs können nicht wiederhergestellt werden.

## Mahlzeit

Standardmässig gibt es drei Mahlzeiten: «Zmorgen», «Zmittag» und «Znacht». Du kannst diese bei Bedarf anpassen.

### Mahlzeit hinzufügen

Klicke auf `Mahlzeit hinzufügen` oberhalb des Menüplans. Gib der Mahlzeit einen Namen und bestätige mit `OK`.

### Mahlzeit umbenennen

Klicke auf die drei Punkte ⋮ neben dem Mahlzeitennamen und wähle `Umbenennen`.

### Mahlzeit verschieben

Bei aktiviertem «Drag & Drop» kannst du die gesamte Mahlzeitenzeile per Drag and Drop neu anordnen.

### Mahlzeit löschen

Klicke auf die drei Punkte ⋮ neben dem Mahlzeitennamen und wähle `Löschen`.

{: .warning }
Beim Löschen einer Mahlzeit werden alle Menüs, geplante Rezepte, Produkte, Materialien und Notizen dieser Mahlzeit gelöscht. Dieser Schritt kann nicht rückgängig gemacht werden.

## Notizen

Du kannst an verschiedenen Stellen Notizen erfassen — z.B. für die Menüverantwortung, einen Geburtstag oder andere hilfreiche Informationen.

![Notiz in der Tagesüberschrift](/docs/event/images/menueplan_header_with_note.png){: width="500"}

Klicke auf die drei Punkte ⋮ in der Menükarte oder auf der Spaltenüberschrift und wähle `Notiz hinzufügen`. Über dasselbe Menü kannst du Notizen ändern (`Notiz anpassen`) oder löschen (`Notiz löschen`).

## Produkte und Materialien

Du kannst einem Menü auch einzelne Produkte und/oder Materialien hinzufügen — z.B. Geburtstagskerzen zu einem Kuchen oder ein paar Früchte für den Zvieri. Hinzugefügte Produkte und Materialien werden direkt in der Menükarte angezeigt und bei der Generierung der [Einkaufs-]({% link docs/event/shoppinglist.md %}) bzw. [Materialliste]({% link docs/event/materiallist.md %}) berücksichtigt.
{::comment}[[shoppinglist]][[materiallist]]{:/comment}

### Hinzufügen

Klicke auf die drei Punkte ⋮ neben dem Menünamen und wähle `Produkt hinzufügen` oder `Material hinzufügen`. Bei der Menge hast du die Wahl zwischen einer absoluten Menge (z.B. 10 Geburtstagskerzen) oder einer Verknüpfung mit der [Mengenberechnung]({% link docs/event/groupconfiguration.md %}) (z.B. 1 Apfel pro Person).
{::comment}[[groupconfiguration]]{:/comment}

### Bearbeiten / Löschen

Klicke auf die drei Punkte ⋮ → `Menü bearbeiten`. Im Dialog kannst du Einträge über das Mülleimer-Symbol löschen oder über das Stift-Symbol die Menge ändern.

## Druckversion

Klicke auf `Druckversion` oberhalb des Menüplans, um den gesamten Menüplan als PDF zu exportieren.
