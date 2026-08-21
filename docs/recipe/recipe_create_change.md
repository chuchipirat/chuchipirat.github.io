---
layout: default
title: Rezept anlegen/ändern
permalink: docs/recipe/create_edit
nav_exclude: false
parent: Rezepte
nav_order: 3
---
# Rezept anlegen und/oder bearbeiten
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

Diese Seite zeigt dir, worauf du achten sollst, wenn du ein neues Rezept anlegst oder ein bestehendes bearbeitest.

{: .note }
Du kannst nur eigene Rezepte ändern, die nicht veröffentlicht wurden. Falls du bei einem veröffentlichten Rezept einen Fehler gefunden hast, ist [hier]({% link docs/recipe/recipe_report_bug.md %}) beschrieben, wie du vorgehen kannst.
{::comment}[[recipe_report_bug]]{:/comment}

## Titel und Bildquelle

Gib dem Rezept den passenden Namen. Unter diesem Namen erscheint es überall, wo du es einfügst.

Wenn du ein Bild einfügen möchtest, kannst du folgendermassen vorgehen:

![Bild-URL kopieren](/docs/recipe/images/copy_recipe_image_url.gif)

- Suche im Internet eine Seite mit einem passenden Bild. Bewährt haben sich [migusto.ch](https://migusto.migros.ch), [fooby.ch](https://fooby.ch), [bettybossi.ch](https://www.bettybossi.ch), [swissmilk.ch](https://www.swissmilk.ch).
- Mache einen Rechtsklick auf das Bild und wähle im Kontextmenü den Eintrag «Bildadresse kopieren» (je nach Browser kann der Menüeintrag leicht anders heissen).
- Füge die kopierte Adresse im Feld «Bildquelle» ein. Wenn die Adresse erkannt wird, wird das Bild umgehend angezeigt.

{: .note-title }
> Wieso kann ich keine eigenen Bilder hochladen?
>
> Aus urheberrechtlichen Gründen kann der chuchipirat keine Rezeptbilder speichern. Die Überprüfung, ob ein hochgeladenes Bild urheberrechtlich geschützt ist, ist nicht möglich. Deshalb wird nur die Möglichkeit angeboten, eine Bildreferenz zu speichern (was rechtlich erlaubt ist).

## Allgemeine Informationen

In diesem Abschnitt gibst du die Eckdaten zum Rezept an:

- **Quelle** — woher das Rezept stammt (URL, Buchtitel mit Seitenzahl, Zeitschrift usw.)
- **Vorbereitung** — Zubereitungszeit in Minuten
- **Koch/Backzeit** — Koch- oder Backzeit in Minuten
- **Menütyp** — wofür sich das Rezept eignet (z.B. Frühstück, Zvieri/Znüni)
- **Geeignet für Outdoor-Küche** — ob das Rezept auch unter vereinfachten Küchenverhältnissen (z.B. im Zeltlager) zubereitet werden kann
- **Hinweis** — ein optionaler Tipp oder Hinweis zum Rezept
- **Tags** — Schlagwörter, die bei der Suche in der [Rezeptübersicht]({% link docs/recipe/recipes_overview.md %}) berücksichtigt werden. Neue Tags fügst du über das `+` hinzu.
{::comment}[[recipes_overview]]{:/comment}

{: .highlight }
Möchtest du das [Rezept veröffentlichen]({% link docs/recipe/recipe_publish.md %}), musst du eine gültige Quelle angeben.
{::comment}[[recipe_publish]]{:/comment}

{: .note-title }
> Wieso kann ich die Diätinfo nicht selber bestimmen?
>
> Die Diätinfo wird anhand der gewählten Zutaten ermittelt. Jede Zutat ist kategorisiert, ob sie für gewisse Diäten (vegetarisch, vegan) und/oder Unverträglichkeiten (z.B. Laktose) geeignet ist. Die Summe aller Zutaten ergibt, ob das Rezept sich für die angezeigten Diäten eignet.

## Zutaten

Hier führst du alle Produkte auf, die für das Rezept benötigt werden. Zuoberst gibst du die Anzahl **Portionen** an, für die das Rezept ausgelegt ist.

Eine Zutat besteht aus folgenden Feldern:

- **Menge** — wie viel davon verwendet wird (kann auch leer bleiben)
- **Einheit** — in welcher Einheit die Menge angegeben ist. Bei Stückzahlen (z.B. 3 Äpfel) kannst du das Feld leer lassen.
- **Zutat** — wähle aus dem Dropdown die passende Zutat. Fange an zu tippen, um die Auswahl zu filtern. Falls die Zutat noch nicht existiert, kannst du eine neue anlegen.
- **Details** — optionale Angabe, wie die Zutat benötigt wird (z.B. «in feinen Streifen»). Diese Information erscheint nur im Rezept und wird nicht in die Einkaufsliste übertragen.

### Kontextmenü und Reihenfolge

Über die drei vertikalen Punkte ⋮ am Ende jeder Zeile öffnest du das Kontextmenü mit folgenden Optionen:

- **Neue Position einfügen** — fügt eine neue Zeile ein
- **Neuer Abschnitt einfügen** — fügt einen Abschnitt zur Gliederung ein
- **Löschen** — entfernt die Zeile
- **Nach oben / unten verschieben** — verschiebt die Zeile

Alternativ kannst du die Reihenfolge per **Drag and Drop** ändern: Klicke eine Zeile an (aber nicht in ein Feld) und ziehe sie mit gedrückter Maustaste an die gewünschte Stelle.

![Zutaten neu anordnen](/docs/recipe/images/rearrange_ingredients.gif)

### Abschnitte

Mit Abschnitten kannst du die Zutaten thematisch unterteilen — zum Beispiel in einem Wähenrezept die Zutaten für den Teig von denen des Belags trennen. So kannst du ein Produkt (z.B. Zucker) mehrmals im Rezept auflisten und in unterschiedliche Abschnitte gruppieren. Abschnitte werden auch in der PDF-Version angezeigt.

![Abschnitt einfügen](/docs/recipe/images/create_section.gif)

### Skalierungsfaktoren

Über den Schalter «Skalierungsfaktoren anzeigen» (rechts neben dem Feld «Portionen») kannst du pro Zutat einen individuellen Skalierungsfaktor hinterlegen. Mögliche Werte sind 0.1 bis 1.0.

{: .note-title }
> Was ist ein Skalierungsfaktor?
>
> {% include_relative _includes/scalingfactor.md %}

## Zubereitung

Beschreibe hier die einzelnen Schritte, die für die Zubereitung nötig sind. Die Zubereitungsschritte werden im Rezept, in der PDF-Version sowie im Abschnitt «Verwendete Rezepte» im Menüplan angezeigt.

Auch hier stehen dir das Kontextmenü ⋮ und Drag and Drop zur Verfügung — genau wie bei den Zutaten. Ebenso kannst du Abschnitte einfügen, um die Schritte zu gliedern.

## Material

Benötigt dein Rezept spezielles Material? Backpapier, ein Spritzbeutel oder Gonfigläser? Hier kannst du das Material hinterlegen. Wähle aus dem Dropdown das gewünschte Material und gib bei Bedarf eine Menge an. Auch hier kannst du Zeilen per Kontextmenü oder Drag and Drop verwalten.

{: .note }
Gib im Dropdown deinen Suchbegriff ein — die Auswahl wird automatisch gefiltert. Falls das gewünschte Material noch nicht existiert, kannst du [ein neues Material anlegen]({% link docs/masterdata/materials.md %}).
{::comment}[[materials]]{:/comment}
