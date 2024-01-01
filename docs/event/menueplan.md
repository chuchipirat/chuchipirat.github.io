---
layout: default
title: Menüplan
nav_exclude: false
has_children: false
nav_order: 3
parent: Anlass
---
# Menüplan
{: .no_toc }

## Inhalt
{: .no_toc .text-delta }

- TOC
{:toc}

---
Die Menüplanung ermöglicht es dir, festzulegen, wann du welche Rezepte kochen möchtest. Dabei kannst du die Portionen planen und auch [Notizen](#notizen), [Produkte](#produkte-und-materialien) sowie [Materialien](#produkte-und-materialien) für einzelne Menüs hinterlegen.

![Leerer Menüplan](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/empty_menueplan.png?raw=true)
_leerer Menüplan_

## Struktur

#### Tage
Für jeden Tag, den du bei der Erstellung angegeben hast, wird eine Spalte im Menüplan angezeigt. Die Anpassung der Tage erfolgt in den [Infos zum Anlass]({% link docs/event/event settings.md %}).
{::comment}[[event settings]]{:/comment}
#### Mahlzeit
Eine Mahlzeit definiert eine bestimmte Essenszeit, standardmässig *Zmorgen*, *Zmittag* und *Znacht*. Du kannst Mahlzeiten [hinzufügen](#mahlzeit-hinzufügen), [löschen](#mahlzeit-l%C3%B6schen), [verschieben](#mahlzeit-verschieben) oder [umbenennen](#mahlzeit-umbenennen).
#### Menü
Ein Menü ist eine Sammlung von Rezepten, die an einem Tag zu einer bestimmten Mahlzeit geplant werden. Eine Mahlzeit kann mehrere Menüs haben.

## Rezepte im Menüplan

### Rezepte hinzufügen
Um ein Rezept im Menüplan hinzuzufügen, kannst du auf die Schaltfläche `Rezept Hinzufügen +` klicken. Es öffnet sich die Rezeptübersicht, in der dir alle öffentlichen Rezepte, deine privaten Rezepte sowie die Rezeptvarianten dieses Anlasses angezeigt werden. 
Falls du Rezepte suchen willst, kannst du dies, indem du einen Suchbegriff eingibst oder du die `Erweiterte Suche` aktivierst. Mehr dazu findest du [hier]({% link docs/recipe/recipes overview.md %}#suche). In der Rezeptübersicht kannst du ein Rezept über das Plus-Symbol dem Menü hinzufügen. Wenn du das Rezept vorher anschauen willst, kannst du das Rezept öffnen und von dort aus über den Button `+Zu Anlass hinzufügen` hinzufügen.

Als Nächstes wirst du gefragt, in welchen Menüs du das Rezept aufnehmen möchtest. Falls du das Rezept an mehreren Tagen/Mahlzeiten planen möchtest, kannst du weitere Menüs anwählen.

![Dialog, für welche Menüs das Rezept geplant wird](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_choose_menue.png?raw=true)

Zum Schluss gibst du an, wie viele Portionen du planst. Dabei hast du zwei Möglichkeiten.

{::comment}[[groupconfiguration]]{:/comment}

#### Variable Mengen abhängig von der Mengenberechnung
Du kannst die Anzahl Portionen mit einer oder mehreren Ernährungsgruppen und Unverträglichkeiten aus der [Gruppeneinstellung]({% link docs/event/groupconfiguration.md %}) verknüpfen. Dies bringt den Vorteil, dass du zu einem späteren Zeitpunkt die Anzahl Portionen pro Gruppe anpassen kannst und die verknüpften Rezepte übernehmen die Anpassung automatisch. Um das gewählte Rezept, so einzuplanen, wähle zuerst eine Ernährungsgruppe, indem du in der oberen Buttonreihe die gewünschte Gruppe anwählst. Danach aktivere die Checkboxen, für die Unverträglichkeitsgruppen. Sobald du eine Checkbox aktivierst, siehst du auf der rechten Seite, wie viele Portionen mit der aktuellen Gruppeneinstellung hinterlegt sind. Du kannst, auch einen Faktor hinterlegen. Falls du zum Beispiel nur die Hälfte der Portionen hinterlegen willst (beispielsweise weil du 2 Spaghettisaucen machst) oder du ausnahmsweise etwas mehr zubereiten möchtest (beispielsweise nach einem Sportblock). Die Anzahl Portionen, die aus der Gruppeneinstellung kommen, werden zum Schluss mit den von dir angegeben Faktor multipliziert. Am Ende der Liste wird angezeigt, für wie viele Portionen das Rezept eingeplant wird.

![Dialog, für welche Menüs das Rezept geplant wird](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_set_portions.png?raw=true)
_Dialog wie ein Rezept für den Freitag, 17.Mai.2024 zum Zmittag eingeplant wird._

#### Fixe Menge
Du kannst auch eine fixe Anzahl Portionen hinterlegen. Diese bleibt auch gleich, wenn du die [Gruppeneinstellung]({% link docs/event/groupconfiguration.md %}) anpasst. Wähle dafür in der oberen Buttonreihe den Eintrag `Fixe Portionen` und hinterlege die Anzahl Portionen, die du planen möchtest.
{::comment}[[groupconfiguration]]{:/comment}

Klicke auf den Button `Hinzufügen` für die Einplanung.
### Eingeplante Portionen ändern
Um die geplanten Portionen eines Rezeptes anzupassen, klicke neben dem Menünamen auf die 3 vertikalen Punkte und wähle aus dem Kontextmenü den Eintrag `Menü bearbeiten`. Klicke in der Menüübersicht auf das Bleistift-Symbol und pass die Menge wie gewünscht an.  


![Menü bearbeiten](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_edit_menue.png?raw=true)
_Auflistung aller zugeordneten Elemente im Menü._

### Rezepte verschieben
Ziehe ein geplantes Rezept mittels Drag-and-drop in ein anderes Menü.

### Rezept löschen
Klicke neben dem Menünamen auf die 3 Punkte und wähle `Menü bearbeiten`. Klicke auf das Abfalleimer-Symbol, um ein Rezept aus dem Menü zu löschen.

{: .highlight }
Wird ein [Rezept gänzlich gelöscht]({% link docs/recipe/recipe structure.md %}#rezept-l%C3%B6schen) (also nicht nur aus dem Menüplan raus), werden in allen Menüplänen die Verknüpfung entfernt. Dabei wird ein Text hinterlassen, damit du siehst, dass das Rezept nicht mehr existiert.

![Gelöschtes Rezept im Menüplan](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_deleted_recipe.png?raw=true)
_Vermerk im Menü, dass das Rezept Tomatenrisotto gelöscht wurde._

## Menü
Das Menü sammelt alle nötigen Rezepte, zusätzliche Produkte und Materialien, die du für die Zubereitung deines Menüs benötigst. Du kannst, dem Menü auch einen Namen geben, dieser wird dann in den diversen Dialogen übernommen und erleichtert die Orientierung. 

### Menü verschieben
Um ein Menü auf eine andere Mahlzeit zu verschieben, kannst du dieses per Drag-and-drop an die gewünschte Stelle ziehen. Gehe mit der Maus an den Rand der Menükarte, drücke die linke Maustaste und ziehe die Karte mit gedrückter Maustaste an die gewünschte Stelle. Lass die linke Maustaste los und die Karte wird an die gewünschte Stelle verschoben.

![Verschiebung eines Menüs](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_move_menue.gif?raw=true)
_Die Menüs zweier Tage tauschen den Platz._

### Menü löschen
Um ein Menü zu löschen, klicke in der entsprechenden Karte auf die 3 Punkte in der oberen rechten Ecke und wähle den Eintrag `Menü löschen` aus dem Kontextmenü.

{: .warning }
> Beachte, dass gelöschte Menüs nicht wiederhergestellt werden können.

# Neues Menü erstellen
Um ein neues Menü zu erstellen, musst du in einer Mahlzeit, die (noch) kein Menü hat auf die das den Text `NEUES MENÜ` klicken. Dadurch wird an dieser Stelle ein neues Menü erstellt. 


![Mahlzeit ohne Menü](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menuplan_create_new_menue.png?raw=true)
_Freitag zum Zmorgen gibt es kein Menü. Mit einem Klick auf den Text NEUES MENÜ wird eine neue Menükarte erstellt._

{: .highlight-title }

> 💡Tipp
> 
> Falls alle Mahlzeiten ein Menü besitzen, kannst du eines an einen Ort verschieben, ein neues Menü an der neuen leeren Stelle erzeugen und danach das zuvor verschobene Menü wieder zurückverschieben. 

## Mahlzeit
Standardmässig gibt es drei Mahlzeiten: _Zmorgen_, _Zmittag_, _Zvieri_. Ändere dies bei Bedarf.

### Mahlzeit hinzufügen
Um eine neue Mahlzeit zu erstellen, klicken in der oberen linke Ecke des Menüplans (oberhalb der ersten Mahlzeit) auf den Button _Mahlzeit hinzufügen_. Gibt deiner Mahlzeit den gewünschten Namen und bestätige mit `OK`.

### Mahlzeit umbenennen

Um den Namen einer bestehenden Mahlzeit zu ändern, klicke in auf die drei Punkte rechts neben dem Mahlzeitennamen und wähle den Eintrag `Umbennen` aus dem Kontextmenü. Gibt deinen gewünschten Namen ein und bestätige mit `OK`.
### Mahlzeit verschieben

Um die Reihenfolge der Menüs zu ändern, kannst du dieses per Drag-and-drop neu anordnen. Gehe mit der Maus auf die Mahlzeitenkarte (ganz rechts im Menüplan), drücke die linke Maustaste und ziehe die Karte mit gedrückter Maustaste an die gewünschte Stelle. Lass die linke Maustaste los und die gesamte Reihe wird an die gewünschte Stelle verschoben.


![Reihenfolge der Menüs ändern](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_move_menue.gif?raw=true)
_Zwei Menüs tauschen die Tage, an denen sie geplant werden._
### Mahlzeit löschen

Wenn du eine Mahlzeit löschen willst, kannst du dies indem du in der Mahlzeitenkarte auf die 3 Punkte klickst und im Kontextmenü den Eintrag `Löschen` wählst.

{: .warning }
> Achtung, löscht du eine Mahlzeit, werden alle Menüs, deren geplante Rezepte, Produkte, Materialien und Notizen gelöscht. Dieser Schritt kann nicht rückgängig gemacht werden!
 
## Notizen
Du kannst an verschiedenen Stellen eine Notiz erfassen. Die kann hilfreich sein, um zum Beispiel die Menüverantwortung, einen Geburtstag oder andere hilfreiche Informationen im Menüplan festzuhalten.


![Überschrift mit Notiz](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_header_with_note.png?raw=true){: width="500px"}  
_Notiz in einer Tagesüberschrift._
### Notiz hinzufügen
Um eine neue Notiz zu erstellen, klicke in der Menükarte oder auf der Spaltenüberschrift auf die 3 Punkte und wähle den Eintrag `Notiz hinzufügen` aus dem Kontextmenü. Gib deine gewünschte Notiz ein und bestätige mit `OK`.

### Notiz ändern/löschen
Um eine Notiz zu löschen oder zu ändern klicke in der entsprechenden Karte auf die 3 Punkte und wähle den gewünschten Eintrag, `Notiz anpassen` oder `Notiz löschen`.

## Produkte und Materialien
Du kannst einem Menü auch einzelne Produkte und/oder Materialien hinzufügen. So kannst du zum Beispiel Geburtstagskerzen zu einem Kuchen hinzufügen und musst dafür das Rezept nicht anpassen. Oder du notierst ein paar Früchte für einen Zvieri. Hinzugefügte Produkte/Materialien werden bei der Generierung der [Einkaufs-]({% link docs/event/shoppinglist.md %}) bzw. [Materialliste]({% link docs/event/materiallist.md %}) berücksichtigt.
{::comment}[[shoppinglist]][[materiallist]]{:/comment}
### Produkte/Material hinzufügen
Um ein Produkt/Material hinzuzufügen, klicke neben dem Menünamen auf die 3 vertikalen Punkte und wähle aus dem Kontextmenü den Eintrag `Produkt hinzufügen`oder `Material hinzufügen` aus. Im nächsten Dialog wählst du, welches Produkt/Material du dem Menü hinzufügen möchtest. Bei der Menge hast du die Möglichkeit, eine absolute Menge einzugeben (bspw. 10 Geburtstagskerzen) oder du verknüpfst die Menge mit der [Mengenberechnung]({% link docs/event/groupconfiguration.md %}) (bspw. 1 Apfel pro Person).
{::comment}[[groupconfiguration]]{:/comment}

### Produkte/Material Bearbeiten/Löschen
Um ein Produkt/Material anzupassen/löschen, klicke neben dem Menünamen auf die 3 vertikalen Punkte und wähle aus dem Kontextmenü den Eintrag `Menü bearbeiten`. Im Dialog hast du nun die Möglichkeit, einzelne Elemente mittels Klick auf das Abfalleimer-Symbol zu löschen oder du änderst die Menge mittels Klick auf das Bleistift-Symbol.
