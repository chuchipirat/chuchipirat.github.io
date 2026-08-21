---
layout: default
title: Einkaufsliste
nav_exclude: false
has_children: false
nav_order: 5
parent: Anlass
---
# Einkaufsliste
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

Die Einkaufsliste wird automatisch anhand der geplanten Rezepte im Menüplan generiert. Die Mengen aller Produkte werden zusammengerechnet und nach [Abteilungen]({% link docs/masterdata/departments.md %}) sortiert — so wie du die Artikel im Laden findest. Du kannst beliebig viele Listen erstellen.
{::comment}[[departments]]{:/comment}

## Liste erstellen

1. Klicke auf `Neue Liste`.
2. Wähle die Menüs aus, die berücksichtigt werden sollen.

![Menüauswahl für die Erstellung einer Einkaufsliste](/docs/event/images/shoppingList_choose_menue.png)

{: .highlight }
Mit den Buttons `Tag auswählen` oder `Alle auswählen` kannst du schnell alle Menüs eines Tages oder des gesamten Anlasses markieren.

{:start="3"}
3. Wähle die **Abteilungen**, die in der Liste erscheinen sollen (z.B. nur «Früchte» und «Gemüse» für einen Marktbesuch). Mit `Alle auswählen` markierst du alle Abteilungen.
4. Gib der Liste einen Namen und bestätige.

### Wie wird die Liste generiert?

Alle Rezepte der gewählten Menüs werden auf die hinterlegten Portionen skaliert. Die skalierten Mengen werden pro Produkt und Einheit gruppiert und summiert. Wo möglich, rechnet der chuchipirat die Mengen in die «Einkaufseinheit» um.

Bei den Materialien werden nur Materialien vom Typ [«Verbrauchsmaterial»]({% link docs/masterdata/materials.md %}#verbrauchsmaterial) automatisch in die Einkaufsliste aufgenommen. [«Gebrauchsmaterial»]({% link docs/masterdata/materials.md %}#gebrauchsmaterial) landet in der [Materialliste]({% link docs/event/materiallist.md %}).
{::comment}[[materials]][[materiallist]]{:/comment}

{: .important-title }
> Wieso kommen einzelne Artikel mehrmals vor?
>
> Wenn ein Produkt in verschiedenen Rezepten mit unterschiedlichen Einheiten hinterlegt ist und diese nicht ineinander umgerechnet werden können (z.B. 4 Stück Rüebli und 200 g Rüebli), werden sie als separate Positionen aufgeführt.

## Aufbau einer Zeile

Die Liste ist nach Abteilungen gegliedert (z.B. Molkerei, Backzutaten, Gewürze). Jede Zeile enthält:

- **Checkbox:** zum Abhaken beim Einkaufen
- **Menge:** berechnete Menge
- **Einheit:** Dropdown mit Einheiten
- **Artikel:** Produktname (Dropdown mit allen bekannten Produkten, akzeptiert auch Freitext)
- **⋮:** Kontextmenü (ändern, löschen, Nachverfolgung)

Über die leere Zeile am Ende jeder Abteilung kannst du Produkte manuell hinzufügen. Wählst du ein bekanntes Produkt aus dem Dropdown, wird es automatisch in die richtige Abteilung einsortiert. Bei Freitext bleibt der Artikel in der gewählten Abteilung und wird alphabetisch eingeordnet.

Über `Abteilung hinzufügen` kannst du weitere Abteilungen zur Liste hinzufügen.

## Bearbeitungsmodus und Einkaufsmodus

Die Liste hat zwei Modi, die du über die Tabs oben umschalten kannst:

- **Bearbeitungsmodus:** alle Felder sind als Eingabefelder dargestellt. Hier bearbeitest du Mengen, Einheiten und Artikel.
- **Einkaufsmodus:** die Eingabefelder werden durch reinen Text ersetzt. So kannst du beim Einkaufen schnell Produkte per Checkbox abhaken, ohne versehentlich etwas zu ändern.

{: .highlight }
Die Liste ist in Echtzeit synchronisiert. Wenn mehrere Personen gleichzeitig einkaufen, sehen alle sofort, was bereits abgehakt wurde.

{: .note }
Damit die Live-Synchronisation funktioniert, müssen alle Geräte mit dem Internet verbunden sein.

## Liste bearbeiten

- **Name/Menüs ändern:** Klicke auf das Stift-Symbol neben dem Listeneintrag.
- **Löschen:** Klicke auf das Mülleimer-Symbol. Gelöschte Listen können nicht wiederhergestellt werden.

## Liste aktualisieren

Wenn du nach der Erstellung etwas am Menüplan änderst, warnt dich der chuchipirat, dass die Einkaufsliste nicht mehr aktuell ist.

![Warnung, dass Einkaufsliste aktualisiert werden muss](/docs/event/images/shoppingList_refresh_needed.png)

Klicke auf `Aktualisieren`, um die Liste neu zu berechnen. Falls du manuell hinzugefügte Artikel hast, wirst du gefragt, ob diese behalten oder entfernt werden sollen.

## Positionen ändern / löschen

Über die drei vertikalen Punkte ⋮ kannst du eine Position ändern, löschen oder die Nachverfolgung öffnen. Bei Doppelerfassungen (gleiches Produkt + Einheit) fragt der chuchipirat, ob die Mengen addiert oder überschrieben werden sollen.

### Produktnachverfolgung

Über `Woher stammt dieses Produkt?` im Kontextmenü zeigt dir der chuchipirat, aus welchen Rezepten und Menüs das Produkt stammt.

## Druckversion

Klicke auf `Druckversion`, um die Einkaufsliste als PDF zu exportieren.
