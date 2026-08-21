---
layout: default
title: Produkte
nav_exclude: false
nav_order: 1
has_children: false
parent: Stammdaten
---
# Produkte
{: .no_toc }

---

Produkte sind der Grundbaustein eines jeden Rezeptes. Ein Produkt stellt immer ein Lebensmittel dar und hat verschiedene Eigenschaften, die den gesamten Planungsprozess unterstützen.

### Abteilung

Die Abteilung bezieht sich auf den Ort, an dem du dieses Produkt im Laden findest. Anhand dieser Information wird die [Einkaufsliste]({% link docs/event/shoppinglist.md %}) sortiert.
{::comment}[[shoppinglist]]{:/comment}

### Einheit

Die Einkaufseinheit beschreibt, in welcher Einheit das Lebensmittel üblicherweise verkauft wird. Bei der Erstellung der Einkaufsliste wird versucht, die Einheit aus dem Rezept in die Einkaufseinheit umzurechnen — damit du im Laden nicht rätseln musst, wie viel 32 Löffel Honig wohl sind.

{: .note }
Für Produkte, die in Stück verkauft werden (z.B. Äpfel), lässt du das Feld «Einheit» leer.

### Unverträglichkeiten

Ein Lebensmittel kann verschiedene Unverträglichkeiten auslösen. Du kannst angeben, ob das Produkt Laktose und/oder Gluten enthält. Diese Information wird genutzt, um Rezepte automatisch zu kategorisieren.

### Produkteigenschaft

Die Produkteigenschaft bestimmt, für welche Diät ein Rezept geeignet ist. Die Optionen sind:

- **ist Fleisch**
- **Vegetarisch**
- **Vegan**

## Neues Produkt anlegen

Beim Erstellen oder Bearbeiten eines Rezeptes suchst du nach einer Zutat, die es noch nicht gibt? Dann erstelle ein neues Produkt:

1. Tippe im Zutat-Dropdown den Namen ein. Wenn kein Produkt mit dem eingegebenen Namen existiert, wähle den Eintrag «... hinzufügen».
2. Es öffnet sich der Dialog «Neue Zutat erstellen».
3. Passe bei Bedarf den Produktnamen an. Verwende immer die Mehrzahlform (z.B. «Äpfel» statt «Apfel»).
4. Wähle die **Abteilung**, in der du das Produkt im Laden suchen würdest.
5. Wähle die **Einheit**, in der das Produkt üblicherweise verkauft wird.
6. Setze die **Unverträglichkeiten** und die **Produkteigenschaft** entsprechend.
7. Klicke auf `Erstellen`.

![Dialog neue Zutat erstellen](/docs/masterdata/images/create_product.png)

{: .important }
Bitte prüfe vor dem Anlegen, ob das Produkt im chuchipirat nicht bereits existiert. Der Produktname sollte keine Marken, Mengen, Einheiten oder Zubereitungsformen enthalten. Produkte, die nicht den Richtlinien entsprechen, können ohne Voranmeldung geändert oder gelöscht werden.

{: .note-title }
> Nicht sicher bei Unverträglichkeiten oder Produkteigenschaft?
>
> Keine Sorge — du kannst die Checkboxen auch leer lassen. Die Community-Leader prüfen neu erfasste Produkte und passen die Einstellungen bei Bedarf an.
