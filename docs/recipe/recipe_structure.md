---
layout: default
title: Rezeptaufbau
permalink: docs/recipe/structure
parent: Rezepte
nav_exclude: false
nav_order: 2
---
# Rezeptaufbau
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

Diese Seite zeigt dir, wie ein Rezept im chuchipirat aufgebaut ist und welche Funktionen dir zur Verfügung stehen.

## Aufbau

### Rezeptname und Bewertung

Zuoberst siehst du den Namen des Rezeptes. Bei öffentlichen Rezepten wird zusätzlich eine Sternebewertung angezeigt. Du kannst mit einem Klick auf die Sterne eine eigene Bewertung abgeben.

Direkt darunter findest du die Aktions-Buttons: `Skalieren`, `Druckversion` und — bei öffentlichen Rezepten — `Fehler melden`.

### Informationen

Hier findest du die wichtigsten Eckdaten zum Rezept:

- **Quelle** — woher das Rezept stammt
- **Portionen** — für wie viele Personen das Rezept ausgelegt ist
- **Zubereitungszeit / Kochzeit / Ruhezeit** — die jeweiligen Zeitangaben
- **Diätinfo** — ob das Rezept vegetarisch, vegan etc. ist (wird automatisch anhand der Zutaten ermittelt)

{: .highlight-title }
> Wieso wird die Zeit nicht angepasst, wenn das Rezept skaliert wird?
>
> Die benötigte Zeit hängt von vielen Faktoren ab (Art der Zubereitung, Ausrüstung, Anzahl Köch\*innen) und lässt sich nicht zuverlässig skalieren. Deshalb zeigt chuchipirat immer die Zeitangaben für die Originalportionen an.

### Tipps & Tags

Hier siehst du Hinweise und Tipps zum Rezept. Die Tags werden bei der Suche in der [Rezeptübersicht]({% link docs/recipe/recipes_overview.md %}) berücksichtigt.
{::comment}[[recipes_overview]]{:/comment}

### Zutaten

Hier siehst du alle benötigten Zutaten mit Mengen und Einheiten. Wurde das Rezept skaliert, werden sowohl die Original- als auch die skalierten Mengen angezeigt.

**Unlogische skalierte Werte?**
Wenn skalierte Werte nicht linear erscheinen, wurde bei der entsprechenden Zutat ein abweichender Skalierungsfaktor hinterlegt.

{: .note-title }
> Was ist ein Skalierungsfaktor?
>
> {% include_relative _includes/scalingfactor.md %}

### Zubereitung

Die Schritt-für-Schritt-Anleitung für die Zubereitung des Rezeptes.

### Material

Hier siehst du, ob spezielles Material benötigt wird (z.B. Spätzlisieb, Backform).

### Kommentare

Bei öffentlichen Rezepten können Nutzer\*innen Kommentare hinterlassen — zum Beispiel Tipps, Erfahrungen oder Anpassungsvorschläge.

## Funktionen

### Skalieren

Die meisten Rezepte sind für 4 Portionen ausgelegt. Mit `Skalieren` kannst du die Mengen auf eine beliebige Portionenzahl hochrechnen.

Dabei können Einheiten automatisch umgerechnet werden — zum Beispiel von Esslöffeln in Milliliter. So musst du nicht 45 Esslöffel Öl abmessen, sondern kannst einfach 675 ml in einen Messbecher abfüllen.

{: .note-title }
> Wie funktioniert die Umrechnung?
>
> Zu jedem Lebensmittel ist eine Einkaufseinheit hinterlegt. Der chuchipirat versucht, die Menge anhand der [Mengenumrechnungen]({% link docs/masterdata/unitconversion.md %}) in diese Einheit umzurechnen.
{::comment}[[unitconversion]]{:/comment}

{: .important-title }
> Skalieren ist nicht immer linear
>
> Beachte, dass beim Skalieren die Zubereitungstexte (enthaltene Mengen) und die Koch-/Backzeit allenfalls nicht mehr stimmen.

### Druckversion

Über `Druckversion` kannst du das Rezept als PDF herunterladen. Möchtest du alle Rezepte deines Menüplans auf einmal herunterladen? Im Abschnitt [Verwendete Rezepte]({% link docs/event/used_recipes.md %}) ist beschrieben, wie das geht.
{::comment}[[used_recipes]]{:/comment}

### Fehler melden

Bei öffentlichen Rezepten kannst du über `Fehler melden` einen Fehler an die Community-Leader melden. Mehr dazu auf der Seite [Rezept Fehler melden]({% link docs/recipe/recipe_report_bug.md %}).
{::comment}[[recipe_report_bug]]{:/comment}

### Zu Anlass hinzufügen

Rufst du die [Rezeptübersicht]({% link docs/recipe/recipes_overview.md %}) aus dem Menüplan heraus auf, kannst du ein Rezept direkt einer Mahlzeit hinzufügen. Wie das geht, ist im Abschnitt [Menüplan]({% link docs/event/menueplan.md %}) beschrieben.
{::comment}[[recipes_overview]][[menueplan]]{:/comment}

### Eigene Variante erstellen

Du kannst von einem Rezept eine Anlass-spezifische Variante erstellen, um es geringfügig anzupassen. Mehr dazu unter [Variante erstellen]({% link docs/recipe/recipe_create_variant.md %}).
{::comment}[[recipe_create_variant]]{:/comment}

### Rezept löschen

Du kannst private Rezepte löschen. Dafür musst du den Namen des Rezeptes eingeben und die Löschung bestätigen.

{: .warning }
Gelöschte Rezepte können nicht wiederhergestellt werden. Löschst du ein Rezept, das in einem Menüplan eingeplant ist, wird bei der entsprechenden Mahlzeit ein Hinweis hinterlassen, dass das Rezept gelöscht wurde.
