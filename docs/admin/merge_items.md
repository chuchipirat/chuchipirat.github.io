---
layout: home
title: Items zusammenführen
permalink: docs/admin/merge_items
nav_exclude: 
parent: System
search_exclude: true
---
# Items zusammenführen
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

{: .intern-title }

> ☠️ Admin-Bereich ☠️
>
>Diese Seite ist für die Community-Leader\*innen und System-Admins.


Wenn viele Benutzer gemeinsam arbeiten, ist es wichtig, Ordnung zu halten. Es kann vorkommen, dass dasselbe Lebensmittel oder Material mehrmals erfasst wird, vielleicht sogar mit leicht unterschiedlichen Namen oder Tippfehlern. Dadurch denkt das System, dass es sich um zwei verschiedene Produkte/Materialien handelt. Diese werden dann getrennt in den Einkaufs-/Materialliste aufgeführt und können nicht zusammengezählt werden.

![Items zusammenführen](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/admin/_images/merge_items.png?raw=true)
## Vorgehen

Um zwei Produkte/Materialien zusammenzuführen, befolge diese Schritte:

1. Wähle, ob du Produkte oder Materialien zusammenführen willst.
2. Wähle im Dropdown-Menü `Produkt A` bzw. `Material A` das Item aus, das du ersetzen möchtest.
3. Wähle im Dropdown-Menü `Produkt B` bzw. `Material B` das Item aus, mit dem du Produkt A ersetzen möchtest.
4. Klicke auf `Items zusammenführen`.

Im Hintergrund wird nun eine Cloud-Funktion ausgeführt, die alle Vorkommnisse (Rezepte, Menüpläne, Einkaufslisten) des Item A durch das Item B ersetzt.

{: .note }  

> Es kann einige Minuten dauern, bis die Cloud-Funktion alles bereinigt hat.