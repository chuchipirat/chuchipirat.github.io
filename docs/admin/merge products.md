---
layout: home
title: Produkte zusammenführen
permalink: docs/admin/merge_products
nav_exclude: 
parent: System
search_exclude: true
---
# Produkte zusammenführen
{: .no_toc }

## Inhalt
{: .no_toc .text-delta }

- TOC
{:toc}

---

{: .intern-title }

> ☠️ Admin-Bereich ☠️
>
>Diese Seite ist für die Community-Leader\*innen und System-Admins.


Wenn viele Benutzer gemeinsam arbeiten, ist es wichtig, Ordnung zu halten. Es kann vorkommen, dass dasselbe Lebensmittel mehrmals erfasst wird, vielleicht sogar mit leicht unterschiedlichen Namen oder Tippfehlern. Dadurch denkt das System, dass es sich um zwei verschiedene Produkte handelt. Diese werden dann getrennt in den Einkaufslisten aufgeführt und können nicht zusammengezählt werden.

![Produkte zusammenführen](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/admin/_images/merge_products.png?raw=true)

## Vorgehen

Um zwei Produkte zusammenzuführen, befolge diese Schritte:

1. Wähle im Dropdown-Menü `Produkt A` das Produkt aus, das du ersetzen möchtest.
2. Wähle im Dropdown-Menü `Produkt B` das Produkt aus, mit dem du Produkt A ersetzen möchtest.
3. Klicke auf `Produkte zusammenführen`.

Im Hintergrund wird nun eine Cloud-Funktion ausgeführt, die alle Vorkommnisse (Rezepte, Menüpläne, Einkaufslisten) des Produkts A durch das Produkt B ersetzt.

{: .note }  

> Es kann einige Minuten dauern, bis die Cloud-Funktion alles bereinigt hat.