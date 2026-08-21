---
layout: default
title: Materialliste
nav_exclude: false
has_children: false
nav_order: 6
parent: Anlass
---
# Materialliste
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

Die Materialliste zeigt dir alle Materialien, die du für deinen Anlass benötigst — z.B. Cakeformen, Spritzbeutel oder Stabmixer, die du allenfalls von zu Hause mitnehmen musst. Du kannst beliebig viele Listen erstellen.

Beim Generieren werden alle Materialien vom Typ [«Gebrauchsmaterial»]({% link docs/masterdata/materials.md %}#gebrauchsmaterial) aus den gewählten Rezepten übernommen. Materialien vom Typ [«Verbrauchsmaterial»]({% link docs/masterdata/materials.md %}#verbrauchsmaterial) landen standardmässig in der [Einkaufsliste]({% link docs/event/shoppinglist.md %}).
{::comment}[[materials]][[shoppinglist]]{:/comment}

{: .note-title }
> Mengenberechnung: Maximum statt Summe
>
> Anders als bei der Einkaufsliste werden Materialmengen **nicht summiert**, sondern es wird jeweils die grösste benötigte Menge übernommen. Grund: Gebrauchsmaterial kann wiederverwendet werden — wenn zwei Rezepte je 2 Cakeformen brauchen, reichen 2 Stück (nicht 4).

## Liste erstellen

1. Klicke auf `Neue Liste`.
2. Wähle die Menüs aus, die für die Generierung berücksichtigt werden sollen.
3. Gib der Liste einen Namen und bestätige.

{: .highlight }
Mit den Buttons `Tag auswählen` oder `Alle auswählen` kannst du schnell alle Menüs eines Tages oder des gesamten Anlasses markieren.

## Aufbau einer Zeile

Jede Zeile in der Materialliste enthält:

- **Checkbox** — zum Abhaken erledigter Positionen
- **Menge** — benötigte Stückzahl
- **Material** — Dropdown mit allen bekannten Materialien. Akzeptiert auch Freitext, falls das Material nicht im Dropdown vorhanden ist.
- **Verantwortlich** — hier kannst du festhalten, welches Teammitglied für dieses Material zuständig ist
- **⋮** — Kontextmenü (ändern, löschen, Nachverfolgung)

{: .note }
Über das Materialfeld werden keine neuen Materialien in der Datenbank angelegt. Wenn du ein Material dauerhaft erfassen möchtest, nutze die [Material-Verwaltung]({% link docs/masterdata/materials.md %}).
{::comment}[[materials]]{:/comment}

## Material manuell hinzufügen

Du kannst jederzeit weitere Materialien von Hand zur Liste hinzufügen — unabhängig vom Materialtyp.

## Liste bearbeiten

- **Name/Menüs ändern:** Klicke auf das Stift-Symbol neben dem Listeneintrag.
- **Löschen:** Klicke auf das Mülleimer-Symbol. Gelöschte Listen können nicht wiederhergestellt werden.

## Liste aktualisieren

Wenn du nach der Erstellung etwas am Menüplan änderst, warnt dich der chuchipirat, dass die Materialliste nicht mehr aktuell ist. Klicke auf `Aktualisieren`, um die Liste neu zu berechnen. Falls du manuell hinzugefügte Materialien hast, wirst du gefragt, ob diese behalten oder entfernt werden sollen.

## Positionen ändern / löschen

Über die drei vertikalen Punkte ⋮ am Ende einer Zeile kannst du eine Position ändern, löschen oder die Nachverfolgung öffnen.

### Produktnachverfolgung

Über `Woher stammt dieses Material?` im Kontextmenü zeigt dir der chuchipirat, aus welchen Rezepten und Menüs dieses Material stammt.

## Druckversion

Klicke auf `Druckversion`, um die Materialliste als PDF zu exportieren.
