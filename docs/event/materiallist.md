---
layout: home
title: Materialliste
nav_exclude: false
has_children: false
nav_order: 6
parent: Anlass
---
# Materialliste
{: .no_toc }
## Inhalt
{: .no_toc .text-delta }

- TOC
{:toc}

---
Mit der Funktion Materialliste kannst du dir eine Liste aller Materialien zusammenstellen, die du für deinen Anlass benötigst. Dies kann nützlich sein, wenn du spezielles Material von zu Hause mitnehmen möchtest, um sicherzustellen, dass du alle benötigten Materialien für deine Rezepte hast.
Wenn du dir eine Liste generieren lässt, werden alle Materialien vom Typ [«Gebrauchsmaterial»]({% link docs/masterdata/material.md %}#gebrauchsmaterial) in die Liste aufgenommen für die Rezepte, die du eingeplant hast (einzeln hinzugefügte Produkte im Menüplan werden ebenfalls berücksichtigt). Dazu hast du die Möglichkeit, weitere Materialien von Hand hinzuzufügen.
Du kannst so viele Materiallisten erstellen, wie du magst.
{::comment}[[material]][[materiallist]]{:/comment}
## Materialliste erstellen
Um eine neue Materialliste zu erstellen, klicke auf den Button `neue Liste`. Im nächsten Dialogfenster wählst du die Menüs, die du für die Generierung der Liste berücksichtigen möchtest.


![Menüauswahl für die Erstellung einer Materialliste](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/materialList_choose_menue.png?raw=true)
_Auswahl der Menüs._

{: .highlight-title }
> 💡Tipp
> 
> Du kannst mit den Buttons `Tag auswählen` oder `Alle auswählen` gleich alle Menüs des Anlasses oder alle Menüs eines Tages auswählen. 

Sobald du die Auswahl bestätigt hast, kannst du der Liste einen Namen geben.
## Wie wird die Materialliste generiert

Für die Generierung der Liste werden alle Rezepte der gewählten Menüs berücksichtigt. Die Rezepte werden auf die hinterlegten Anzahl-Portionen skaliert. Die skalierten Mengen werden dann in der Liste aufgenommen. Dabei werden nur Materialien vom Typ «Gebrauchsmaterial» berücksichtigt. Wenn ein Material in mehreren Rezepten vorkommt, wird jeweils verglichen, welches Rezept wie viele Stücke von diesem Material benötigt. Es wird jeweils die Maximal-Anzahl übernommen. Anders als in der Einkaufsliste werden die Mengen nicht summiert, sondern der Eintrag mit der grösseren Menge wird in die Liste übernommen. Die Überlegung dahinter ist, dass Materialien wiederverwendet werden können und daher nur für die Zubereitung eines bestimmten Rezepts in der angegebenen Anzahl erforderlich sind. 

Die Materialien vom Typ [«Verbrauchsmaterial»]({% link docs/masterdata/material.md %}#verbrauchsmaterial) landen standardmässig in der [Einkaufsliste]({% link docs/event/shoppinglist.md %}). Du hast die Möglichkeit, weitere Materialien (unabhängig vom Typ) manuell zur Liste hinzuzufügen. 
  {::comment}[[shoppinglist]][[material]]{:/comment}
## Material zur Liste hinzufügen

Um einzelne Materialien hinzuzufügen, klicke auf die Schaltfläche `Material hinzufügen`. Im nächsten Fenster kannst du das benötigte Material auswählen. Falls es das gewünschte Material bisher nicht gibt, kannst du auch ein neues anlegen.

## Listenname ändern
Du kannst den Namen der Liste ändern, indem du neben dem Listeneintrag auf den Bleistift klickst und den Namen nach Belieben änderst.
## Liste löschen
Um eine generierte Liste zu löschen, klicke auf das Abfalleimer-Symbol. Beachte, dass gelöschte Listen nicht wiederhergestellt werden können. Falls du eine Liste versehentlich löschst, musst du sie neu erstellen.

## Liste aktualisieren  

Wenn du nach der Erstellung der Liste etwas am Menüplan änderst, kann es sein, dass die Mengen und Materialien in der Materialliste nicht mehr stimmen. Der chuchipirat warnt dich mit einer Meldung, dass eine Aktualisierung notwendig ist.


![Warnung, dass Materialliste aktualisiert werden muss. ](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/materialList_refresh_needed.png?raw=true)
_Warnung, dass die Einkaufsliste aktualisiert werden muss._

Klicke dazu auf den Button `Aktualisieren`. Wenn du in der zu aktualisierenden Liste manuell hinzugefügte Materialien hast, fragt dich der chuchipirat, ob du diese Einträge behalten möchtest oder ob diese mit der Aktualisierung gelöscht werden sollen. Wähle hierfür den entsprechenden Button. Das System berechnet danach die Materialliste anhand des Menüplans neu.

## Positionen löschen/ändern  

Um eine Position zu löschen oder die Menge anzupassen, klicke bei der entsprechenden Position auf die 3 vertikalen Punkte und wähle im Kontextmenü den gewünschten Eintrag `Ändern` oder `Löschen` aus.

## Produktnachverfolgung

Wenn du dich fragst, warum ein bestimmtes Material auf der Materialliste steht, kannst du mit der Produktnachverfolgung auf einfache Weise herausfinden, wie es den Weg auf die Materialliste geschafft hat. Klicke auf die 3 vertikalen Punkte und wähle im Kontextmenü den Eintrag `Woher stammt dieses Material?` aus. aus. Der chuchipirat listet dir nun jedes Rezept und Menü aus, das dieses Material verwendet.

## Materialliste drucken

Um die Materialliste als PDF zu exportieren, wähle die Liste und klicke auf den Button `Druckversion`.