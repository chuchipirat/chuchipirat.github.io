---
layout: home
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

Die folgende Seite zeigt dir, wie das Rezept im chuchipirat aufgebaut ist und welche Möglichkeiten du von hast.

## Aufbau

Das Rezept ist in fünf Abschnitten gegliedert.

### Rating

Im Abschnitt mit dem Namen siehst du bei öffentlichen Rezepten ein Rating. Du kannst mit einem Klick auf die Sterne eine eigene Bewertung abgeben.

### Informationen

Im Abschnitt Informationen siehst du grundlegende Information wie die Zeit für die Zubereitung, die Quelle sowie die Diät-Infos. Die Diät-Infos werden automatisch ermittelt anhand der benötigten Zutaten.
Im Abschnitt _Tipps & Tags_ siehst du Hinweise/Tipps. Die Tags werden bei der Suche in der [Rezeptübersicht]({% link docs/recipe/recipes_overview.md %}) berücksichtigt.
{::comment}[[recipes_overview]]{:/comment}

{: .highlight-title }

> Wieso wird die Zeit nicht angepasst, wenn das Rezept skaliert wird?
> 
> Wir haben viel darüber nachgedacht, wie wir Zubereitungszeiten skalieren können, aber bisher keine passende Lösung gefunden. Die Zeit, die für das Kochen benötigt wird, hängt von verschiedenen Faktoren ab, wie der Art der Zubereitung, der Anzahl der Personen, die kochen, und der verfügbaren Ausrüstung. Die Kochzeit ist nicht überall gleich. Während die Zubereitungszeit für Pasta in etwa 11 Minuten beträgt, ist die Zubereitung von Gerichten wie Omeletten, die pro Portion gekocht werden, unterschiedlich. Auch die Zubereitungsdauer variiert. Zum Beispiel dauert es genauso lange, einen Teig mit einer Teigmaschine für 20 Personen herzustellen wie für 4 Personen (vorausgesetzt, die Maschine kann das bewältigen). Das Schälen von Rüebli hingegen dauert proportional zur Menge. Es ist also nicht möglich, die Zubereitungszeiten global zu skalieren. Anstatt ungenaue Informationen anzuzeigen, zeigen wir lieber die Zeit an, die für die Originalmengen im Rezept benötigt wird.


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
Rufst du die [Rezeptübersicht]({% link docs/recipe/recipes_overview.md %}) aus dem Menüplan heraus aus, kannst du das angezeigte Menü auch gleich einer bestimmten Mahlzeit deines Anlasses hinzufügen. Wie das geht, ist [hier]({% link docs/event/menueplan.md %}) beschrieben. 
{::comment}[[recipes_overview]][[menueplan]]{:/comment}
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
Du kannst von einem Rezept eine Anlass-spezifische Variante erstellen. Das kann hilfreich sein, wenn du ein bestehendes Rezept (geringfügig) anpassen willst. Mehr Informationen findest du [hier]({% link docs/recipe/recipe_create_variant.md %}){::comment}[[recipe_create_variant]]{:/comment}

### Druckversion

Über diese Funktion kannst du das Rezept als PDF herunterladen. Möchtest du alle Rezepte, welche du in deinem Menüplan hast als PDF herunterladen? Im Abschnitt [Verwendete Rezepte]({% link docs/event/used_recipes.md %}) ist beschrieben, wie das geht.
{::comment}[[used_recipes]]{:/comment}

### Rezept löschen

Du hast die Möglichkeit, private Rezept zu löschen. Um die Löschung durchzuführen, musst du den Namen des Rezeptes eingeben und die Löschung bestätigen.

{: .warning }
Gelöschte Rezepte können nicht wiederhergestellt werden und sind für immer verloren. Löschst du ein Rezept, welches in einem Menüplan eingeplant wurde, wird bei der entsprechenden Mahlzeit ein Hinweis hinterlassen, dass das dazugehörige Rezept gelöscht wurde.