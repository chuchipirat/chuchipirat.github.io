---
layout: home
title: Menüplan
nav_exclude: false
has_children: false
nav_order: 3
parent: Anlass
---
#todo #todo_languagetool #todo_image 
# Menüplan
{: .no_toc }

## Inhalt
{: .no_toc .text-delta }

- TOC
{:toc}

---

Im Menüplan bestimmst du wann du welches Rezept kochen willst. Dabei hinterlegst du auch wie viele Portionen du planst. Auch hast du die Möglichkeit [Notizen](#notizen), einzelne [Produkte](#produkte-und-materialien) und/oder [Materialien](#produkte-und-materialien) für einzelne Menüs zu planen. 

![Leerer Menüplan](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/empty_menueplan.png?raw=true)
_leerer Menüplan_

## Struktur

Der Menüplan ist folgendermassen aufgebaut:

##### Tage
Für jeden Tag, der du bei der Erstellung angegebene hast, wird eine Spalte angezeigt. Falls du die Tage anpassen willst, kannst du dies in den [Infos zum Anlass]({% link docs/event/event settings.md %}).

##### Mahlzeit
Eine Mahlzeit beschreibt eine bestimmte Essenszeit. Standardmässig werden im Menüplan die Mahlzeit *Zmorgen*, *Zmittag* und *Znacht* eingefügt. Du kannst auch weitere [Mahlzeit hinzufügen](#mahlzeit-hinzufügen), [Mahlzeiten löschen, verschieben](#mahlzeit-verschiebenl%C3%B6schen) oder [bestehende umbenennen](#mahlzeit-umbenennen).

##### Menü
Ein Menü ist eine Sammlung von Rezepten, welche an einem Tag zu einer bestimmten Mahlzeit geplant wird. Eine Mahlzeit kann mehrere Menüs haben (standardmässig hat eine Mahlzeit ein Menü). Das Menü bietet somit die Möglichkeit Rezepte zu gruppieren.

## Rezepte im Menüplan

### Rezepte hinzufügen
Um ein Rezept im Menüplan hinzuzufügen, kannst du auf die Schaltfläche _Rezept Hinzufügen +_ klicken. Es öffnet sich die Rezeptübersicht, in der dir alle öffentlichen Rezepte, deine privaten Rezepte sowie die Rezeptvarianten dieses Anlasses angezeigt werden. 
Falls du Rezepte suchen willst, kannst du dies indem du einen Suchbegriff eingibst oder du aktivierst die Erweiterte Suche. Mehr dazu findest du [hier]({% link docs/recipe/recipes overview.md %}#suche). 
Aus der Rezeptübersicht hast die Möglichkeit ein Rezept über das grosse Plus hinzuzufügen. Wenn du das Rezept vorher anschauen willst, kannst du das Rezept öffnen und von dort aus über den Button _+Zu Anlass hinzufügen_ hinzufügen.

Als nächstes wirst du gefragt, in welche Menüs du das Rezept aufnehmen möchtest. Der Tag den du zu beginn gewählt hast, ist bereits vorgewählt. Falls du das Rezept an mehreren Tagen/Mahlzeiten planen möchtest, kannst du weitere Menüs anwählen.

![Dialog, für welche Menüs das Rezept geplant wird](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_choose_menue.png?raw=true)

Zum Schluss gibst du an, wie viele Portionen du planst. Dabei hast du zwei Möglichkeiten.

{::comment}[[groupconfiguration]]{:/comment}

- Du kannst die Anzahl Portionen mit einer oder mehreren Ernährungsgruppen und Unverträglichkeiten aus der [Gruppeneinstellung]({% link docs/event/groupconfiguration.md %}) verknüpfen. Dies bringt den Vorteil, dass du zu einem späteren Zeitpunkt die Anzahl Portionen pro Gruppe anpassen kannst und die verknüpften Rezepte übernehmen die Anpassung automatisch. Um das gewählte Rezept so einzuplanen, wähle zuerst eine Ernährungsgruppe indem du in der oberen Buttonreihe die gewünschte Gruppe anwählst. Danach aktivere die Checkboxen, für die Unverträglichkeitsgruppen. Sobald du eine Checkbox aktivierst, siehst du auf der rechten Seite, wieviele Portionen mit der aktuellen Gruppeneinstellung hinterlegt sind. Du kannst, auch einen Faktor hinterlegen. Falls du zum Beispiel nur die Hälfte der Portionen hinterlegen willst (Beispielsweise weil du 2 Spaghettisaucen machst) oder du ausnahmsweise etwas mehr zubereiten möchtest (Beispielsweise nach einem Sportblock). Die Anzahl Portionen, die aus der Gruppeneinstellung kommen, werden zum Schluss mit den von dir angegeben Faktor multipliziert. Zuunterst siehst du was die gewählten Einstellung für einen Einfluss auf die geplanten Portionen ausüben. 

![Dialog, für welche Menüs das Rezept geplant wird](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/event/_images/menueplan_set_portions.png?raw=true)
_Dialog wie ein Rezept für den Freitag, 17.Mai.2024 zum Zmittag eingeplant wird. Das gewählte Rezept wird….. #todo _

{::comment}[[groupconfiguration]]{:/comment}
- Du kannst auch eine fixe Anzahl Portionen hinterlegen. Diese bleibt auch gleich, wenn du die [Gruppeneinstellung]({% link docs/event/groupconfiguration.md %}) anpasst. Wähle dafür in der oberen Buttonreihe den Eintrag _Fixe Portionen_ und hinterlege die Anzahl Portionen, die du planen möchtest.

Mit einem Klick auf den Button _Hinzufügen_ wird die Einplanung in den Menüplan übernommen.
### Eingeplante Portionen ändern
### Rezepte verschieben

### Rezept löschen

{: .highlight }
Wird ein [Rezept gänzlich gelöscht]({% link docs/recipe/recipe structure.md %}#rezept-l%C3%B6schen) (also nicht nur aus dem Menüplan raus), werden in allen Menüplänen die Verknüpfung entfernt. Dabei wird ein Text hinterlassen, damit du siehst, dass das Rezept nicht mehr existiert.

{: .placeholder }
Bild gelöschtes Rezept

## Menü

Das Menü sammelt alle nötigen Rezepte, zusätzliche Produkte und Materialien, die du für die Zubereitung deines Menüs benötigst. Du kannst, dem Menü auch einen Namen geben, dieser wird dann in den diversen Dialogen übernommen und erleichtert die Orientierung. 
### Menü verschieben

Um ein Menü auf eine andere Mahlzeit zu verschieben, kannst du dieses per Drag and Drop an die gewünschte Stelle ziehen. Gehe mit der Maus an den Rand der Menükarte, drücke die linke Maustaste und ziehe die Karte mit gedrückter Maustaste an die gewünschte Stelle. Lass die linke Maustaste los und die Karte wird an die gewünschte Stelle verschoben.

#todo_image : GIF wie Menü verschoben wird
### Menü löschen

Um ein Menü zu löschen, klicke in der entsprechenden Karte auf die 3 Punkte in der oberen rechten Ecke und wähle den Eintrag _Menü löschen_ aus dem Kontexmenü. Um sicherzustellen, dass du das Menü wirklich löschen willst, wirst du gefragt ob das Menü wirklich löschen willst. Bestätige die Frage, wenn dies deine Absicht ist. 

> {: .warning }
> Beachte, dass gelöschte Menüs nicht wiederhergestellt werden können.

# Neues Menü erstellen

Um ein neues Menü zu erstellen, musst du in einer Mahlzeit, die (noch) kein Menü hat auf die das ???? klicken. Dadurch wird an dieser Stelle ein neues Menü erstellt. 

{: .highlight-title }

> 💡Tipp
> 
> Falls alle Mahlzeiten ein Menü besitzen, kannst du eines an einen Ort verschieben, ein neues Menü an der neuen leeren Stelle erzeugen und danach das zuvor verschobene Menü wieder zurückverschieben. 

## Mahlzeit

Standardmässig hat dein Menüplan drei Mahlzeiten: _Zmorgen_, _Zmittag_, _Zvieri_. Falls du dies ändern möchtest, kannst du dies mit den folgenden Funktionalitäten.
### Mahlzeit hinzufügen

Um eine neue Mahlzeit zu erstellen, klicken in der oberen linke Ecke des Menüplans (oberhalt der ersten Mahlzeit) auf den Button _Mahlzeit hinzufügen_. Gibt deiner Mahlzeit den gewünschten Namen und bestätige mit _OK_.

### Mahlzeit umbenennen

Um den Namen einer bestehende Mahlzeit zu ändern, klicke in auf die drei Punkte rechts neben dem Mahlzeitennamen und wähle den Eintrag _Umbennen_ aus dem Kontexmenü. Gibt deinen gewünschten Namen ein und bestätige mit _OK_.
### Mahlzeit verschieben

Um die Reihenfolge der Menüs zu ändern, kannst du dieses per Drag and Drop neu Anordnen. Gehe mit der Maus auf die Mahlzeitenkarte (ganz rechts im Menüplan), drücke die linke Maustaste und ziehe die Karte mit gedrückter Maustaste an die gewünschte Stelle. Lass die linke Maustaste los und die gesamte Reihe wird an die gewünschte Stelle verschoben.

#todo_image GIF wie Mahlzeit verschoben wird
### Mahlzeit löschen

Wenn du eine Mahlzeit löschen willst, kannst du dies indem du in der Mahlzeitenkarte auf die 3 Punkte klickst und im Kontextmenü den Eintrag _Löschen_ wählst. Um ein versehentliches löschen zu erschweren, wirst du gefragt ob du sicher bist. Wenn du die Mahlzeit löschen willst bestätige das mit einem Klick auf den Button _OK_. 

> {: .warning }
> Achtung, löscht du eine Mahlzeit, werden alle Menüs, deren geplante Rezepte, Produkte, Materialien und Notizen gelöscht. Dieser Schritt kann nicht rückgängig gemacht werden!
> 
## Notizen

## Produkte und Materialien
### Produkte/Material hinzufügen

  

**... verschieben/löschen**

