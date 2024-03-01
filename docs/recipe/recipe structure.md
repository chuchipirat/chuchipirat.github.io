---
layout: home
title: Rezeptaufbau
permalink: recipe/structure
parent: Rezepte
nav_exclude: false
nav_order: 2
---
# Rezeptaufbau
{: .no_toc }
## Inhalt
{: .no_toc .text-delta }

- TOC
{:toc}

---

Die folgende Seite zeigt dir, wie das Rezept im chuchipirat aufgebaut ist und welche Möglichkeiten du von hast.

## Aufbau

Das Rezept ist in fünf Abschnitten gegliedert.

### Rating

Im Abschnitt mit dem Namen siehst du bei öffentlichen Rezepten ein Rating. Du kannst mit einem Klick auf die Sterne eine eigene Bewertung abgeben.

### Informationen

Im Abschnitt Informationen siehst du grundlegende Information wie die Zeit für die Zubereitung, die Quelle sowie die Diät-Infos. Die Diät-Infos werden automatisch ermittelt anhand der benötigten Zutaten.
Im Abschnitt _Tipps & Tags_ siehst du Hinweise/Tipps. Die Tags werden bei der Suche in der [Rezeptübersicht]({% link docs/recipe/recipes overview.md %}) berücksichtigt.
{::comment}[[recipes overview]]{:/comment}
### Zutaten

Im Zutatenabschnitt siehst du alle benötigten Zutaten sowie deren Mengen (und Einheiten). Wurde das Rezept, skaliert siehst du die original- sowie die skalierten Mengen.

**Unlogische skalierte Werte?**  
Werden die Werte skaliert und scheinen diese nicht linear zu sein? Dann wurde bei der entsprechenden Zutat ein abweichender Skalierungsfaktor hinterlegt.

{: .note-title }

> Was ist ein Skalierungsfaktor?
> 
> {% include_relative _includes/scalingfactor.md %}

### Zubereitung

Der Abschnitt Zubereitung beschreibt die nötigen Schritte, welche für das Gelingen des Rezeptes nötig sind.

### Material

In diesem Block siehst du, ob du spezielles Material benötigst, um das Rezept zuzubereiten.

## Funktionen

### Zu Anlass hinzufügen
Rufst du die [Rezeptübersicht]({% link docs/recipe/recipes overview.md %}) aus dem Menüplan heraus aus, kannst du das angezeigte Menü auch gleich einer bestimmten Mahlzeit deines Anlasses hinzufügen. Wie das geht, ist [hier]({% link docs/event/menueplan.md %}) beschrieben. 
{::comment}[[recipes overview]][[menueplan]]{:/comment}
### Skalieren

Die meisten Rezepte sind für 4 Portionen. Du kannst im Rezept über den entsprechenden Button (oder Menüeintrag) das Rezept skalieren. Damit hast du die Möglichkeit, die benötigten Mengen hochzurechnen.

Beim Skalieren hast du die Möglichkeit, Einheiten umrechnen zu lassen. So wird zum Beispiel versucht, die Menge in Ess- und Teelöffeln in das metrische System umzurechnen. Dies ist vor allem dann praktisch, wenn du nicht 45 Esslöffel Öl abmessen, sondern einfach 675 ml in einen Messbecher abfüllen möchtest.

{: .note-title }

> Wie funktioniert das?
> 
>  Mit Lebensmittel ist eine Einkaufseinheit hinterlegt. Der chuchipirat versucht nun Anhand der Mengenumrechnung die Menge in die Einkaufseinheit umzurechnen. Dafür bedient er sich der hinterlegten [Mengenumrechnungen]({% link docs/masterdata/unitconversion.md %}).
{::comment}[[unitconversion]]{:/comment}

{: .important-title }

> 🧐 skalieren ist nicht immer linear
> 
> Beachte, dass eine Skalierung einige Tücken mit sich bringt. So können die Zubereitungstexte allenfalls nicht mehr stimmen (enthaltene Mengen) und auch die Koch-/Backzeit kann allenfalls variieren.

### Eigene Variante erstellen
Du kannst von einem Rezept eine Anlass-spezifische Variante erstellen. Das kann hilfreich sein, wenn du ein bestehendes Rezept (geringfügig) anpassen willst. Mehr Informationen findest du [hier]({% link docs/recipe/recipe create variant.md %}){::comment}[[recipe create variant]]{:/comment}

### Druckversion

Über diese Funktion kannst du das Rezept als PDF herunterladen. Möchtest du alle Rezepte, welche du in deinem Menüplan hast als PDF herunterladen? Im Abschnitt [Verwendete Rezepte]({% link docs/event/used recipes.md %}) ist beschrieben, wie das geht.
{::comment}[[used recipes]]{:/comment}

### Rezept löschen

Du hast die Möglichkeit, private Rezept zu löschen. Um die Löschung durchzuführen, musst du den Namen des Rezeptes eingeben und die Löschung bestätigen.

{: .warning }
Gelöschte Rezepte können nicht wiederhergestellt werden und sind für immer verloren. Löschst du ein Rezept, welches in einem Menüplan eingeplant wurde, wird bei der entsprechenden Mahlzeit ein Hinweis hinterlassen, dass das dazugehörige Rezept gelöscht wurde.