---
layout: home
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

Die folgende Seite zeigt dir auf, was du achten sollst, wenn du ein neues Rezept anlegst oder ein bestehendes änderst.

{: .note }
Du kannst nur eigenen Rezepte ändern, die nicht veröffentlicht wurde. Falls du bei einem veröffentlichten Rezept einen Fehler gefunden hast, ist [hier]({% link docs/recipe/recipe_report_bug.md %}) beschrieben, wie du vorgehen kannst.  {::comment}[[recipe_report_bug]]{:/comment}

## Titel und Bildquelle

Gib dem Rezept den passenden Namen. Unter diesem Namen erscheint es überall, wo du es einfügst.

Wenn du ein Bild einfügen möchtest, kannst du folgendermassen vorgehen.

![Bild-URL kopieren](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/recipe/_images/copy_recipe_image_url.gif?raw=true)

- Suche im Internet eine Seite mit einem passenden Bild. Bewährt haben sich [migusto.ch](https://migusto.migros.ch), [fooby.ch](https://fooby.ch), [bettybossi.ch](https://www.bettybossi.ch), [swissmilk.ch](https://www.swissmilk.ch).
- Mache einen Rechtsklick auf das Bild und wähle im Kontextmenü den Eintrag "_Bildadresse kopieren_" (💡 je nach Browser, kann der Menüeintrag leicht anders heissen).
- Füge die kopierte Adresse (diese ist im Zwischenspeicher), im Feld Bildquelle ein.
  Wenn die Adresse erkannt wird, wird das Bild umgehend angezeigt.

{: .note-title }

> Wieso kann ich keine eigenen Bilder hochladen?
>  
> Aus Urheberrechtlichen-Gründen kann der chuchipirat keine Rezeptbilder speichern. Die Überprüfung, ob ein hochgeladenes Bild urheberrechtlich geschützt ist, ist nicht möglich. Deswegen wird nur die Möglichkeit angeboten, eine Bildreferenz zu speichern (was rechtlich erlaubt ist).

## Allgemeine Informationen

Gibt in diesem Abschnitt die Quelle und die Zeiten an, welche für die Zubereitung benötigt werden (in Minuten). Falls die Quelle keine Internetseite ist, sondern ein Buch, gibt den Buchtitel und die Seitenzahl an.

Unter Menütyp kannst du angeben, wofür sich das Rezept eignet. Ist es ideal für das Frühstück und/oder vielleicht doch Zvieri/Znüni? Mit dem Schalter _Geeignet für Outdoor-Küche_ gibst du an, ob das Rezept auch unter vereinfachten Küchenverhältnissen (beispielsweise in einem Zeltlager) kochbar ist. Mit diesen Angaben kann in der erweiterten Suche der [Rezeptübersicht]({% link docs/recipe/recipes_overview.md %}) das passende Rezept schneller gefunden werden.  {::comment}[[recipes_overview]]{:/comment}

{: .highlight }
💡 Bitte beachte: Möchtest du das [Rezept veröffentlichen]({% link docs/recipe/recipe_publish.md %}) musst du eine gültige Quelle angeben.  {::comment}[[recipe_publish]]{:/comment}

{: .note-title }

> Wieso kann ich die Diät Info nicht selber bestimmen?
>
> Die Diät Info wird anhand der gewählten Zutaten ermittelt. Jede Zutat ist kategorisiert, ob sie für gewisse Diäten (Vegetarisch, Vegan) und/oder Unverträglichkeit (bspw. Laktose) geeignet ist. Die Summe aller Zutaten ergibt schlussendlich, ob das Rezept sich für die angezeigten Diäten eignet oder eben nicht.

## Zutaten

Bei den Zutaten kannst du alle Produkte aufführen, welche für das Rezept benötigt werden.  Eine Zutat besteht aus den folgenden Feldern.

- **Menge**  
  Wie viel wird davon verwendet, du kannst das Feld auch leer lassen.
- **Einheit**  
  In welcher Einheit ist die angegebene Menge. Wenn es sich dabei um Stück handelt (Beispiel 3 Äpfel), kannst du das Feld leer lassen.
- **Zutat**
  Wähle aus dem Dropdown-Menü die Zutat aus. Tipp: Fange an zu tippen und alle Zutaten, die textlich mit deiner Eingabe übereinstimmen, werden angezeigt. Falls es die Zutat im Dropdown nicht gibt, kannst du eine [neue Zutat] anlegen.
- **Details**  
  Dieses Feld kannst du nutzen, um zu definieren, wie die Zutat benötigt wird (zum Beispiel _in feinen Streifen_). Diese Information ist nur auf dem Rezept ersichtlich und wird nicht in die Einkaufsliste übertragen.

Über die drei vertikalen Punkte ⋮, hast du die Möglichkeit, die gewählte Position zu löschen, einen  Abschnitt einzufügen oder die Position zu verändern.

### Reihenfolge der Zutaten bestimmen

Falls du die Reihenfolge der Zutaten ändern willst, kannst du das mittels Drag and Drop. Bewege die Maus über die Position, klicke die Position an (aber nicht in ein Feld), und ziehe die Position (mit gedrückter Maustaste) an die gewünschte Stelle. Sobald du die Maustaste loslässt, wird die Position an die gewünschte Position eingefügt. Alternativ kannst du das auch über die 3 vertikalen Punkte ⋮ und as Kontextmenü erzielen.

![Zutaten neu anordnen](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/recipe/_images/rearrange_ingredients.gif?raw=true)

### Skalierungsfaktoren

Du hast die Möglichkeit, die Skalierungsfaktoren einzublenden. Sobald diese eingeblendet sind (dies geht über den Schalter rechts von dem Feld _Portionen_), kannst du pro Zutat diese ändern. Dabei sind alle Zahlen zwischen 0.1 - 1.0 möglich.

{: .note-title }

> Was ist ein Skalierungsfaktor?
> 
> {% include_relative _includes/scalingfactor.md %}

## Zubereitung

Im Abschnitt Zubereitung kannst du beschreiben, welche einzelnen Schritte nötig sind, um das Rezept zuzubereiten. Damit kannst du die Kochbücher und zu Hause lasen. Diese Angaben werden auf die PDF-Version des Rezeptes sowie auf im Abschnitt _Verwendete Rezepte_ im Menüplan angezeigt.

Auch hier hast du über die 3 vertikalen Punkte ⋮ , die gewählte Position zu löschen, eine neue Position oder Abschnitt einzufügen. Die Positionen können ebenfalls mittels Drag and Drop verschoben werden. Wie das geht, ist im Abschnitt [Reihenfolge der Zutaten bestimmen]({% link docs/recipe/recipe_create_change.md %}#reihenfolge-der-zutaten-bestimmen) beschrieben.

## Abschnitt

Mit einem Abschnitt kannst du die Zutaten und/oder die Zubereitungsschritte unterteilen. So kannst du beispielsweise in einem Wähenrezept die Zutaten für den Teig von denen des Belags trennen. Dies hilft, das Rezept zu gliedern und während des Kochens schneller den Überblick zu behalten. So kannst du ein Produkt (etwa Zucker) mehrmals im Rezept auflisten und in unterschiedliche Abschnitte gruppieren (Teig, Guss)
Abschnitte werden auch auf der PDF-Version angezeigt. Einen Abschnitt fügst du über die 3 Punkte am Ende der Position ein. 

![Abschnitt einfügen](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/recipe/_images/create_section.gif?raw=true)

## Material

Benötigt dein Rezept spezielles Material? Backpapier, ein Spritzbeutel oder Gonfiglässer? Hier kannst du das Material hinterlegen. Wähle hierfür aus dem Dropdown das gewünschte Material. Falls sinnvoll, kannst du auch eine Menge hinterlegen.

{: .note }
Du kannst im Dropdownfeld suchen, in dem du deinen Begriff eingibst. Die Auswahl wird automatisch angepasst mit den Materialien, die deinem Suchbegriff entsprechen. Falls das gewünschte Material noch nicht existiert, kannst du [ein neues Material anlegen]({% link docs/masterdata/materials.md %})  {::comment}[[materials]]{:/comment}


