---
layout: page
title: Release Notes
nav_exclude: false
nav_order: 9
has_children: 
permalink: release_notes
---
{: .no_toc }
## Inhalt
{: .no_toc .text-delta }

- TOC
{:toc}

---

Hier findest du detaillierte Informationen zu den neuesten Versionen unserer Anwendung. Wir arbeiten ständig daran, den chuchipirat zu verbessern und neue Funktionen hinzuzufügen, um deine Planung und Organisation von Anlässen noch einfacher und effizienter zu gestalten.

In den nachfolgenden Abschnitten kannst du die Veröffentlichungshistorie durchgehen, um zu erfahren, welche neuen Features, Verbesserungen und Fehlerkorrekturen in jeder Version enthalten sind. Wir empfehlen, regelmässig einen Blick auf die Release Notes zu werfen, um stets auf dem neuesten Stand zu bleiben und das Beste aus dem chuchipirat herauszuholen.

Vielen Dank für deine Unterstützung und dein [Feedback](mailto:hallo@chuchipirat.ch?subject=Mein%20Feedback%20zum%20chuchipirat) – sie sind für uns von unschätzbarem Wert, um den chuchipirat zu einer noch besseren Erfahrung für dich zu machen!

---

# 1.0.0
Go-live: 25.03.2024
* Bereitstellung der App - Go-live 🎉

## 1.0.4
Go-live: 24.11.2024
* Bugfix [#153](https://github.com/gcettuzz/chuchipirat/issues/153): Im Navigationsmenü, war bei dem Eintrag «Anlässe» nur das Icon als Link klickbar. Der Link wurde nun auf das ganze Listenelement erweitert.
* Bugfix [#155](https://github.com/gcettuzz/chuchipirat/issues/155): Wurde bei einem gespeicherten Rezept nachträglich die Menge eines Materials gelöscht, führte dies unter Umständen zu einem Fehler. 
* Bugfix [#156](https://github.com/gcettuzz/chuchipirat/issues/156): Das Profil konnte ohne Anzeigenamen gespeichert werden. Das führte beim Erstellen einer Rezeptvariante zu einem Fehler. 
* Bugfix [#161](https://github.com/gcettuzz/chuchipirat/issues/161): Fehler bei der Skalierung von Zutaten mit einem Skalierungsfaktor ungleich 1. Die Formel für die Skalierung von Zutaten wurden angepasst.  
* Bugfix [#167](https://github.com/gcettuzz/chuchipirat/issues/167): Fehler bei der Anzeige der Total Portionen im Dialog _Für wen planst du das Rezept ein?_, falls eine Einplanung geändert wird und eine Ernährungsgruppe vorausgewählt ist. 
* Bugfix [#164](https://github.com/gcettuzz/chuchipirat/issues/164): Mehr Feature als Bug 😉. Ist die Postion im Rezept beispielsweise in TL und die produktspezifische Umrechnung in TL wird bei erfolgloser Umrechnung noch versucht, die Position in EL umzurechnen und danach nochmals in das metrische System umzurechnen. 
* Bugfix [#166](https://github.com/gcettuzz/chuchipirat/issues/166): Der Seitenumbruch beim Export der Einkaufsliste führte unter gewissen Umständen zu leeren Seiten. Dieser Fix behebt dies.
* Bugfix [#172](https://github.com/gcettuzz/chuchipirat/issues/172): Registriert sich eine Person neu beim chuchipirat, werden die Einstellungen und Statistikdaten erst erzeugt, wenn die E-Mail-Adresse durch die Person bestätigt wurde. 
* Bugfix [#175](https://github.com/gcettuzz/chuchipirat/issues/175): Rezeptvarianten, die im Menüplan erstellt wurden, konnten durch den\*die Autor\*in geändert werden. Dies wurde geändert, dass alle Crew-Mitglieder Rezeptvarianten auch ändern können.
* Bugfix [#178](https://github.com/gcettuzz/chuchipirat/issues/178): Beim Hinzufügen  von Produkten zum Menüplan, wurde teilweise die falsche Einheit übernommen.
* Bugfix [#181](https://github.com/gcettuzz/chuchipirat/issues/181): Beim Hochladen von Bildern, kam es teilweise zu Fehlern. Wird nun ein Bild hochgeladen (Anlass oder Userprofil), wird neu eine Sanduhr angezeigt bis das Hochladen erfolgreich war. 
 
## 1.0.3 
Go-live: 04.05.2024
* Passwort vergessen Link wird nun bei Falscheingabe des Passwortes angezeigt.
* Möglichkeit deine Notiz in einem Menü über das Kontextmenü zu löschen
* Bei der Abmeldung aus dem chuchipirat, wird das Navigationsmenü nicht mehr angezeigt.
* Neuer Menüeintrag `Spenden`. Damit kann jederzeit der Twintcode aufgerufen werden. 
* Fehler im Menüplan, bei dem Hinzufügen von Produkten/Materialien wurde behoben.
* Auf dem Startbildschirm werden nun mehr Feedeinträge angezeigt.
* Links in der Fusszeile gehen alle in einem neuen Tab auf. 
* Möglichkeit Systemmeldungen zu setzen (Admin-Bereich).
* Beim erfassen eines neuen Produktes wird geprüft, ob es ähnlich klingende Produkte gibt. Eine Liste mit möglichen Übereinstimmungen wird angezeigt um Doubletten zu vermeiden.

## 1.0.2
Go-live: 15.04.2024
* Erweiterung des klickbaren Bereich im Navigationsmenü.
* Korrektur eines Fehlers im Menüplan (Produkt = `undefined`) und Anpassung des Korrekturprogramm, um ein Produkt zu einem Material umzuwandeln.
* Korrektur der Cloud-FX um den Text eines Produktes in allen Objekten nachzuziehen. 
* Korrektur um die Quittung einer Spende zu generieren.
* Neues Korrekturprogramm, um falsch erfasste Materialien in Produkte umzuwandeln.
* Neues Korrekturprogramm, um doppelte Materialien zusammenzuführen. 

## 1.0.1
Go-Live: 27.03.2024
* Diverse Bugfixes und Layout-Anpassungen


