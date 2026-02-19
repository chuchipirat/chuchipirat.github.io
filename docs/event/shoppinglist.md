---
layout: home
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
Im Reiter Einkaufsliste kannst du dir automatisch Einkaufslisten generieren lassen. Dabei wird anhand der geplanten Menüs im Menüplan die Mengen der genutzten Produkte zusammengetragen und in einer Einkaufsliste aufgelistet. Sortiert nach den Abteilungen, in denen du die Artikel im Laden findest.

## Einkaufsliste erstellen
Um eine neue Einkaufsliste zu erstellen, klicke auf den Button `Neue Liste`. Im nächsten Dialogfenster wählst du die Menüs, die du für die Generierung der Einkaufsliste berücksichtigen möchtest.

![Menüauswahl für die Erstellung einer Einkaufsliste](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/shoppingList_choose_menue.png?raw=true)
_Auswahl der Menüs._

{: .highlight-title }
> 💡Tipp
> 
> Du kannst mit den Buttons `Tag auswählen` oder `Alle auswählen` gleich alle Menüs des Anlasses oder alle Menüs eines Tages auswählen. 

Als nächstes, kannst du die Abteilungen wählen, die für die Einkaufsliste berücksichtig werden. Auch hier kannst du alle Abteilungen mit dem Button `Alle auswählen` selektieren.

Sobald du die Auswahl bestätigt hast, kannst du der Liste einen Namen geben.

### Wie wird die Einkaufsliste generiert?
Für die Generierung der Liste werden alle Rezepte der gewählten Menüs berücksichtigt. Die Rezepte werden auf die hinterlegten Anzahl-Portionen skaliert. Die skalierten Mengen werden dann in der Liste aufgenommen und nach Produkt und Einheit gruppiert und zusammen summiert. Wenn die Zwiebeln zum Beispiel in mehreren Rezepten vorkommen, werden alle Mengen zusammengefügt und in der Einkaufsliste als eine Position angezeigt. Wo immer möglich werden die Mengen in die «Einkaufseinheit» umgerechnet.
Bei den Materialien werden nur die Materialien vom Typ [Gebrauchsmaterial]({% link docs/masterdata/materials.md %}#gebrauchsmaterial) automatisch in die Einkaufsliste aufgenommen. Die anderen landen in der [Materialliste]({% link docs/event/materiallist.md %}). Selbstverständlich hast du die Möglichkeit, ein Material vom Typ Gebrauchsmaterial manuell in die Einkaufsliste hinzuzufügen.
  {::comment}[[materials]][[materiallist]]{:/comment}

{: .important-title } 
> 🧐 Wieso kommen einzelne Artikel mehrmals in der Liste vor? 
> 
> Wenn ein Produkt in verschiedenen Rezepten mit unterschiedlichen Einheiten hinterlegt wird und diese nicht ineinander konvertiert werden können, werden diese in der Einkaufsliste nicht auf eine Position reduziert. Wenn ein Rezept beispielsweise 4 Rüebli benötigt und ein anderes 200 g, so können diese beiden unterschiedliche Einheiten (Stück und g) nicht vereinheitlicht werden.

## Produkte hinzufügen
Um einzelne Produkte hinzuzufügen, klicke auf die Schaltfläche `Artikel hinzufügen`. Im nächsten Fenster kannst du das gewünschte Produkt auswählen. Du kannst auch eine Menge und Einheit hinterlegen. Wenn es bereits einen Eintrag in der Einkaufsliste mit diesem Produkt und Einheit gibt, wird der chuchipirat dich fragen, ob du die neue Menge dazuzählen oder den bestehenden Listeneintrag mit der neuen Menge überschreiben möchtest.

## Liste ändern
Du kannst den Namen der Liste und die ausgewählten Menüs ändern, indem du neben dem Listeneintrag auf den Bleistift klickst und den Namen und/oder die ausgwählten Menüs nach Belieben änderst.
## Liste löschen
Um eine generierte Liste zu löschen, klicke auf das Abfalleimer-Symbol. Beachte, dass gelöschte Listen nicht wiederhergestellt werden können. Falls du eine Liste versehentlich löschst, musst du sie neu erstellen.
## Liste aktualisieren
Wenn du nach der Erstellung der Liste etwas am Menüplan änderst, kann es sein, dass die Mengen und Artikel in der Einkaufsliste nicht mehr stimmen. Der chuchipirat warnt dich mit einer Meldung, dass eine Aktualisierung notwendig ist.

![Warnung, dass Einkaufsliste aktualisiert werden muss. ](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/shoppingList_refresh_needed.png?raw=true)
Warnung, dass die Einkaufsliste aktualisiert werden muss._

Klicke dafür auf den Button `Aktualisieren`. Wenn du in der zu aktualisierenden Liste manuell hinzugefügte Artikel hast, fragt dich der chuchipirat, ob du diese Einträge behalten möchtest oder ob diese mit der Aktualisierung gelöscht werden sollen. Wähle hierfür den entsprechenden Button. Das System berechnet danach die Einkaufsliste anhand des Menüplans neu.
## Positionen löschen/ändern
Um eine Position zu löschen oder die Menge anzupassen, klicke bei der entsprechenden Position auf die 3 vertikalen Punkte und wähle aus dem Kontextmenü den gewünschten Eintrag `Ändern`oder `Löschen`aus.

## Mit der Liste Einkaufen
Wenn du nun einkaufen gehst, hast du zwei Möglichkeiten. Du kannst die Liste als PDF exportieren und mit der Papier-Liste im Laden stehen. Oder du öffnest die Einkaufsliste auf deinem Gerät (Mobiltelefon, Tablet, Laptop) und klickst auf die Checkbox, um ein Produkt abzustreichen. Wenn du mit mehreren Personen einkaufst, ist die Liste zwischen allen verbundenen Geräten synchron. Deine Freunde sehen daher, was du bereits abgestrichen hast.

{: .note }
> Damit das Live-Einkaufen funktioniert, muss das entsprechende Gerät auch mit dem Internet verbunden sein.

### Produktnachverfolgung
Wenn du im Laden stehst und dich fragst, warum ein bestimmtes Produkt auf der Einkaufsliste steht, kannst du mit der Produktnachverfolgung auf einfache Weise herausfinden, wie es den Weg auf die Einkaufsliste geschafft hat. Klicke dafür auf die 3 vertikalen Punkte und wähle im Kontextmenü den Eintrag `Woher stammt dieses Produkt?` aus. Der chuchipirat listet dir nun jedes Rezept und Menü aus, das dieses Produkt verwendet.

### Einkaufsliste drucken
Um die Einkaufsliste als PDF zu exportieren, wähle die Liste und klicke auf den Button `Druckversion`.