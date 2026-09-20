---
layout: default
title: Release Notes
nav_exclude: false
nav_order: 9
has_children: false
permalink: release_notes
---
# Release Notes
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

Hier findest du alle Änderungen am chuchipirat. Die neueste Version steht zuoberst.

## 2.0.6 — 20.09.2026

In diesem Update haben wir einige Fehler behoben, die in seltenen Fällen zu Abstürzen oder unklaren Fehlermeldungen geführt haben. Vor allem laden die Rezeptübersicht und die Rezeptsuche im Menüplan jetzt viel schneller, auch bei schlechter Verbindung. Ausserdem ist die Startseite etwas schneller geworden und die App verbindet sich nach einer Unterbrechung jetzt selbst wieder. Für System-Admins gibt es neue Hilfsmittel.

### Neue Funktion

**Deploy-Check für System-Admins**
Unter System gibt es neu den Deploy-Check. Er zeigt, ob gerade ein Lager läuft und wer in den letzten Minuten etwas geändert hat, damit neue Versionen nicht mitten in der Arbeit veröffentlicht werden. Mehr dazu findest du im [Deploy-Check]({% link docs/admin/deploy_readiness.md %}).

### Bugs

**Rezept- und Menüplan-Ansicht konnte abstürzen**
Wenn eine Diät oder Intoleranz nachträglich aus der Gruppenkonfiguration eines Anlasses gelöscht wurde, konnte die Anzeige des Menüplans (z.B. in der Rezeptansicht) abstürzen, falls noch ein Menüplan-Eintrag auf diese gelöschte Diät/Intoleranz verwies. Die Stelle zeigt jetzt stattdessen "Diät gelöscht" bzw. "Intoleranz gelöscht" an.

**Einkaufs-, Material- oder Verwendete-Rezepte-Liste aktualisieren konnte abstürzen**
Wurde eine Mahlzeit aus dem Menüplan gelöscht, auf die eine bestehende Liste noch verwies, konnte das erneute Generieren dieser Liste abstürzen. Die gelöschte Mahlzeit wird jetzt einfach übersprungen.

**Menüplan speichern schlug selten fehl**
Wenn zwei Personen (oder zwei geöffnete Tabs) den Menüplan fast gleichzeitig speicherten, konnte das Speichern in seltenen Fällen mit einem Fehler abbrechen. Gleichzeitige Speicherungen werden jetzt korrekt nacheinander verarbeitet.

**Veralteter Anlass-Link zeigte eine technische Fehlermeldung**
Ein sehr alter, nicht mehr gültiger Link zu einem Anlass führte zu einer kryptischen Fehlermeldung statt der erwarteten "Anlass nicht gefunden"-Meldung. Behoben.

**Rezeptsuche fand Varianten nicht immer**
Eine Rezeptvariante ohne Tags liess sich in der Suche nicht über ihren Variantennamen finden. Jetzt wird der Variantenname immer mitgesucht.

### Verbesserungen

**Rezeptübersicht und Rezeptsuche laden schneller**
Die Rezepte erscheinen jetzt sofort und laden beim Scrollen nach, statt dass du warten musst, bis alle geladen sind. Das merkst du vor allem bei schlechter Verbindung, zum Beispiel im Lager. Das gilt für die Rezeptübersicht und für die Rezeptsuche im Menüplan (dort wird erst geladen, wenn du die Suche öffnest). Auch die Suche selbst ist besser geworden:

* Sie findet Rezepte auch, wenn du Akzente weglässt («hornli» findet «Hörnli»).
* Du kannst mehrere Wörter eingeben, die Reihenfolge spielt keine Rolle.
* Suche und Filter gelten für alle Rezepte, nicht nur für die, die schon angezeigt werden.
* Öffnest du ein Rezept und gehst zurück, sind Suche, Filter und deine Position in der Liste wieder da.

Mehr dazu unter [Rezeptübersicht]({% link docs/recipe/recipes_overview.md %}).

**Startseite lädt schneller**
Die Vorschaubilder der heutigen Rezepte auf der Startseite werden jetzt in einer einzigen Abfrage statt einzeln nacheinander geladen.

**Automatische Wiederverbindung nach Unterbrechung**
Wenn du die App länger im Hintergrund hattest (z.B. Tab gewechselt, Laptop im Standby) oder die Internetverbindung kurz weg war, verbindet sich die Live-Synchronisation (Menüplan, Gruppenkonfiguration usw.) jetzt automatisch wieder. Bisher musste man dafür manuell auf "Erneut versuchen" klicken.

**Klarere Meldung bei abgelaufener Sitzung**
Läuft deine Anmeldung während der Nutzung ab (z.B. nach längerer Inaktivität), zeigt dir die App jetzt eine verständliche Meldung ("Deine Sitzung ist möglicherweise abgelaufen...") mit einem Button zum direkten Neuladen der Seite — statt einer unklaren technischen Fehlermeldung ohne Hinweis, was zu tun ist.

**Mail-Konsole**
Der Abmelde-Footer lässt sich für Nachrichten an einzelne Personen ausschalten, zum Beispiel für eine persönliche Antwort. Bei einem Versand an eine Rolle bleibt er immer aktiv. Ausserdem ist der Titel der Mail neu optional. Mehr dazu in der [Mail-Konsole]({% link docs/admin/mailconsole.md %}).

**Datenintegrität**
Anlässe ohne Zeitscheibe lassen sich auf der Seite Datenintegrität jetzt löschen. Neu gibt es dort auch die Prüfung «Events ohne Köch:innen». Zu jedem Anlass siehst du vorher, was darin steckt, und «Alle löschen» erfasst nur leere Anlässe. Ausserdem zeigen die neuen Prüfungen «Rezept-Zutaten ohne Produkt» und «Rezept-Materialien ohne Material», welche Rezepte nachgebessert werden sollten. Mehr dazu unter [Datenintegrität]({% link docs/admin/data_integrity.md %}).

---
## 2.0.5 — 07.09.2026
Dieser Release behebt weitere Fehler, die mit der V.2.0.0 entstanden sind.
### Bugs
**Rezepte**
* Der Rezept-Editor konnte in seltenen Fällen mit einer weissen Seite abstürzen – beim Speichern oder während des Bearbeitens einer Zutat, wenn die Zutatenliste intern inkonsistent geworden war (auch beim Anlegen einer Variante). Behoben; die Liste wird
  jetzt beim Laden und Speichern automatisch bereinigt.

**Einkaufsliste**
* Im PDF-Export waren die Artikel innerhalb einer Abteilung nicht alphabetisch sortiert wie in der App – behoben.

**Produkte & Materialien** 
* Beim Umwandeln eines Materials in ein Produkt wurden die im Dialog gewählten Eigenschaften (Fleisch / Vegetarisch / Vegan sowie Laktose / Gluten) nicht übernommen – alle so erstellten Produkte waren «Fleisch» ohne Unverträglichkeiten. Behoben.

**Anlässe**
* Administrator:innen können jetzt – z.B. für Support – die Einkaufsliste, die Materialliste und die «Verwendeten Rezepte» eines Anlasses einsehen und bearbeiten, auch ohne selbst als Koch/Köchin des Anlasses eingetragen zu sein (wie beim übrigen Anlass-Inhalt bereits der Fall).

---
## 2.0.4 — 06.09.2026
Dieser Release behebt weitere Fehler, die mit der V.2.0.0 entstanden sind. 
### Neue Funktion
- Gestaffelte Spenden-Meldungen im Feed: Spenden werden im Feed jetzt je nach Betrag mit einem passenden Text gefeiert — von der Schatztruhe bis zur Legende der sieben Meere. 🏴‍
- Klarer Hinweis bei Verbindungsproblemen: Bricht die Live-Verbindung ab (z.B. schwacher Empfang im Lager), zeigt die App neu einen Hinweis „Verbindung wird wiederhergestellt …". Gelingt die automatische Wiederverbindung nicht, erscheint „Live-Aktualisierung nicht möglich" mit einem Button „Erneut versuchen".

### Bugs     
**Einkaufsliste**
* Ein neu hinzugefügter Artikel konnte sofort wieder verschwinden und war danach auf keinem Gerät sichtbar. Ursache war eine Kollision der internen Zeilen-Kennungen zwischen  verschiedenen Listen – behoben. 
* Beim Eintippen einer Menge und anschliessendem Tab (Wechsel ins nächste Feld) sprang der Cursor aus dem Feld – behoben, der Fokus bleibt jetzt erhalten.
* Nach der Meldung «Artikel wurde automatisch in den Abschnitt … verschoben» erschien der Artikel kurzzeitig in zwei Abschnitten – behoben.
* Positionen liessen sich nicht zuverlässig bearbeiten oder löschen und derselbe Artikel tauchte teils mehrfach auf, wenn zwei Personen dieselbe Liste offen hatten – behoben. Änderungen werden jetzt sofort und konfliktfrei gespeichert.
* Eine laufende Eingabe wird nicht mehr überschrieben, wenn gleichzeitig jemand anderes die
  Liste ändert.
* Darstellung im Bearbeitungsmodus auf dem Smartphone verbessert (Mengen- und Einheitenfeld waren zu schmal).

**Materialliste**
* Änderungen anderer Köch\*innen (Menge, Koch-Zuweisung) werden jetzt live angezeigt – bisher erst nach einem Neuladen. 
* Editieren und Löschen von Positionen funktioniert jetzt zuverlässig (gleiche Verbesserung wie bei der Einkaufsliste).

**Rezepte**
* Der Rezept-Editor stürzte in seltenen Fällen ab, wenn Zutaten oder Zubereitungsschritte inkonsistent gespeichert waren – behoben. 

**Menüplan**
* Der automatische Sprung zum heutigen Tag im Menüplan konnte in Einzelfällen zu einem Absturz führen – behoben.

**Produkte & Materialien**
* Wird versucht, ein Produkt oder Material zu löschen, das noch in einem Menüplan verwendet wird, zeigt die App jetzt eine verständliche Fehlermeldung statt einer kryptischen Meldung.
* Ein Material in ein Produkt umzuwandeln schlug komplett fehl, wenn das Material noch in einer Materialliste verwendet wurde – behoben. (Admin / Community Leader)

**Allgemein**
* Der Feedback-Knopf (rundes Symbol unten rechts) öffnete das Feedback-Formular nicht mehr – behoben.

---
## 2.0.3 — 30.08.2026
Dieser Release behebt einige Fehler, die mit der V.2.0.0 entstanden sind. Zudem wurden alle Referenzen zu Firebase entfernt. 
### Bugs

**Einkaufsliste**
* Einen Artikel per Auswahlliste einer anderen Abteilung zuordnen führte zu einem Absturz – behoben.
* Listen mit einer angefangenen, aber noch nicht fertig ausgefüllten Position (z.B. nur eine Menge eingetippt) liessen sich nicht speichern – behoben.
* Das Kontextmenü («⋮») und das Löschen eines Artikels konnten abstürzen, wenn die Liste sich gleichzeitig durch eine andere Person änderte – behoben.

**Menüplan**
* Ein Menüplan liess sich in seltenen Fällen nicht speichern, wenn durch einen Doppelklick ein Mahlzeitentyp doppelt angelegt wurde – behoben, betroffene Pläne speichern jetzt wieder.

**Rezepte**
* Der Rezept-Editor konnte mit einer weissen Seite abstürzen – behoben.
* Klarere Hinweise beim Speichern eines Rezepts, wenn Pflichtangaben fehlen (Portionen, Variantenname), statt einer allgemeinen Fehlermeldung.

**Anlässe & Profil**
* Einige Personen konnten ihre Anlässe, die Anlassübersicht oder ihr Profil nicht laden – behoben.
* Beim Einladen einer Köchin/eines Kochs über eine unbekannte E-Mail-Adresse erscheint jetzt der konkrete Hinweis statt einer allgemeinen Fehlermeldung.
* Läuft die Anmeldung während des mehrschrittigen «Neuer Anlass»-Assistenten ab, erscheint jetzt ein klarer Hinweis, sich neu anzumelden.

**Passwort & E-Mail ändern**
* Hinweise wie «Das neue Passwort muss sich vom alten unterscheiden» werden jetzt sauber angezeigt.

**Stabilität**
* Verbesserte Echtzeit-Aktualisierung bei schwankender Internetverbindung (Anlass, Menüplan, Einkaufs- und Materiallisten verbinden sich nach einem Unterbruch selbstständig neu).

---

## 2.0.2 — 26.08.2026
Behebung diverser kleinerer Fehler und wenige kleine neue Feature.

### Neue Funktionen
* Möglichkeit für Opt-Out von Newsletter über da Profil und über Fusszeilenlink im Mail
* Sauberes Tracking von den Unterseiten im Menüplan über Umami

### Bugs
* Automatisches Re-Subscribe von Realtimelistener, bei Verlust der Verbindung.
* Fehlerbehebung, wenn mit veraltetem Cache versucht wird auf die Datenbank zuzugreifen.
* Bei hinzufügen von bestehenden Produkten in der Einkaufsliste wird nun gefragt ob der neue Eintrag hinzugefügt (Addition) oder Ersetzt werden soll.
* Fehler beim Speichern im Menüplan, falls mit halben Portionen gerechnet wurde.
* Fehler bei hinzufügen von Materialien, wenn keine Menge gewählt.
* Fehlerhafte Anzeige von PDF-Einkaufslisten, wenn nur ein Artikel in der Liste ist.

---

## 2.0.0 — 21.08.2026

Chuchipirat läuft neu auf einer komplett neuen Infrastruktur. Die Datenbank wurde von Firebase auf Supabase/PostgreSQL migriert — schneller, sicherer und zukunftsfähig. Neben dem technischen Umbau gibt es zahlreiche neue Funktionen und Verbesserungen.

### Neue Funktionen

* Anlass kopieren: Anlässe lassen sich neu kopieren. So kannst du die Planung eines vergangenens Jahres kopieren und erneut verwenden. Siehe auch [Anlass-Übersicht]({% link docs/event/overview.md %}) {::comment}[[overview]]{:/comment}
* Spenden-System: Komplett neues Spenden-Management mit Payrexx-Integration, Spendenquittung als PDF, Spendenziel-Widget und Spendenmöglichkeit nach Anlass-Abschluss.
* Koch-Zuweisung in der Materialliste: Materialien können nun einzelnen Köch*innen zugewiesen werden.           
*  Statistiken auf Startseite und Profil: Plattform-KPIs auf der Startseite und persönliche Statistiken (Anlassvarianten, Kommentare, Bewertungen) im Profil.
* Feed-System: Aktivitäts-Feed mit automatischen Einträgen für Rezeptveröffentlichungen, Anlass-Erstellung, neue Produkte/Materialien, Bewertungen und mehr.  
* Bei öffentliche Rezepten können Kommentare hinterlassen werden. 
* Rezepte können im Menüplan mit mehreren Gruppen verknüpft werden. 
* Anfragen-System: Neues Anfragen-System für Rezeptveröffentlichungen und Fehlermeldungen mit Status-Stepper, Kommentaren und Changelog.                                           
* Impressum-Seite: Neue rechtliche Informationsseite.     
* Rezept-Kommentare im Tages-Digest: Die tägliche Zusammenfassung enthält neu auch Rezeptkommentare. (Community Leader / Admin)                                                                            
* Rezept privat setzen: Veröffentlichte Rezepte können aus der Admin-Übersicht direkt wieder auf privat gesetzt werden. (Community Leader / Admin)                                                                 
* Qualitätssicherung für Produkte und Materialien: Neue QA-Seiten mit automatischer Erkennung von Duplikaten, verdächtigen Namen, fehlenden Typen und Plural/Singular-Varianten. Inklusive Zusammenführen, Konvertieren und Synonym-Verwaltung. (Community Leader / Admin)            
* Cron-Jobs: Automatische E-Mails für Tages-Digest, Anlass-Rückblick und Support-User-Bereinigung. (Admin)   
* Während eines Anlasses, werden auf dem Home-Bildschirm, die nächsten zu kochenden Rezepte angezeigt (Quicklink).   
* Einkaufsliste: Bei der Generierung können nun bestimmte Abteilungen ausgewählt werden. [#176](https://github.com/gcettuzz/chuchipirat/issues/176)
* Menüplan: Die Tagesüberschriften bleiben beim Scrollen sichtbar. [#180](https://github.com/gcettuzz/chuchipirat/issues/180)
* Einkaufsliste: Bei der Aktualisierung einer bestehenden Einkaufsliste werden die Markierungen der Checkboxen beibehalten. Abgeänderte Mengen werden angezeigt. [#171](https://github.com/gcettuzz/chuchipirat/issues/171)
* Einkaufs- und Materialliste: Freitextfelder können erfasst werden, ohne dass dafür ein neues Produkt/Material angelegt werden muss. [#174](https://github.com/gcettuzz/chuchipirat/issues/174)
* Menüplan: Unter gewissen Umständen kann der Menüplan inkonsistent werden. Mit einem Klick auf [Konsistenzcheck]({% link docs/event/event_settings.md%}#men%C3%BCplan-konsistenzcheck) können gewisse Fehler nun selbstständig behoben werden. [#193](https://github.com/gcettuzz/chuchipirat/issues/193) {::comment}[[event_settings#Menüplan-Konsistenzcheck]]{:/comment}

### Verbesserungen

* PDF-Exporte: Alle PDFs (Rezept, Menuplan, Materialliste, Einkaufsliste, Verwendete Rezepte) haben ein neues, einheitliches Design mit Theme-Akzentfarbe.
* Spenden-UI: Dynamische Kostenaufschlüsselung, FAQ-Link und TWINT-Empfehlungsdialog vor der Zahlung.           
* Startseite: 2-Spalten-Layout mit Rezeptkarten-Grid, Stats-Sidebar und Leer-Zuständen für alle Sektionen.      
* Passwort-Sicherheit: Stärkere Validierung bei Registrierung und Passwort-Änderung.               
* Hilfe-Links: Alle Seiten haben nun einen direkten Link zum Helpcenter.                                        
* SEO: Open-Graph-Tags, Twitter-Cards, JSON-LD-Strukturdaten und Sitemap für öffentliche Seiten.                
* Mail-Konsole: Bestätigungsdialog vor Massenversand, Empfänger-Chips, Editor/Vorschau nebeneinander, Entwurf-Speicherung und Template-Auswahl. (Community Leader / Admin)
* Google Analytics wurde entfernt. Neu wird [Umami](https://umami.is/) eingesetzt. Eine datenschutzorientierte, quelloffene (Open-Source) Alternative zu Google Analytics.

### Fehlerbehebungen

* Portionenberechnung: Fix-Portionen werden korrekt in die Gesamtsumme eingerechnet, TOTAL-Modus und PER_PORTION-Modus berechnen Mengen richtig.
* Gelöschte Rezepte im Menuplan verursachen keinen Fehler mehr beim Klicken.                                    
* Willkommens-E-Mail wird nun zuverlässig nach der E-Mail-Bestätigung versendet.

### Wartung

Diverse technische Aktualisierungen für mehr Stabilität und Sicherheit.

* Datenbank-Migration: Kompletter Wechsel von Firebase/Firestore auf Supabase/PostgreSQL mit Row-Level Security, 44 Tabellen, 161 RLS-Policies und 36 Funktionen.                                                               
* Sicherheits-Audit: Ownership/Rollen-Guards auf alle RPC-Funktionen, Rate-Limiting, XSS-Schutz via DOMPurify und gehärtete Input-Validierung.                                                                                
* Analytics: Wechsel von Firebase Analytics auf Umami — datenschutzfreundlich, cookie-frei, mit Core Web Vitals Monitoring.                                                                                                     
* Sentry-Upgrade: Aktualisierung auf die neueste Sentry-Version für verbessertes Fehler-Tracking.
* Edge Functions: Alle serverseitigen Funktionen (E-Mail, Webhooks, Cron-Jobs) laufen neu als Supabase Edge Functions (Deno).                                                                                               
* Code-Refactoring: Grosses Refactoring des gesamten Codes — Named Exports, TypeScript-Konvertierung, Sentry statt console.log, Clean-Code-Konventionen.                                                                     
* Hosting: Wechsel von Firebase Hosting auf Coolify (Self-Hosted auf Hetzner). 2 Umgebungen:  TEST / PROD.

<details markdown="block">
<summary>Technische Details</summary>

  * Upgrade auf Latest Release-Stände:                                                                            
    * React: 17 → 19                                                                                              
    * React Router: 5 → 7                                                                                         
    * MUI Material: v5 → v7                                                                                       
    * Firebase: 10 → 12.9 (Legacy, wird in einer zukünftigen Version entfernt)                                    
    * Tooling: CRA → Vite                                                                                         
    * Node.js: 16 → 20        

</details>

---

## 1.1.0 — 30.03.2026

### Fehlerbehebungen

* Rezepte mit fix eingeplanten Portionen wurden in der Einkaufsliste unter gewissen Umständen nicht berücksichtigt. [#188](https://github.com/gcettuzz/chuchipirat/issues/188)

### Wartung

Diverse technische Aktualisierungen für mehr Stabilität und Sicherheit.

<details markdown="block">
<summary>Technische Details</summary>

* Upgrade der Firebase-API auf Version 10.9.0. Der Wechsel erforderte einen kompletten Umbau der Kommunikation zwischen App und Datenbank. [#125](https://github.com/gcettuzz/chuchipirat/issues/125)
* Einbau von [Sentry](https://sentry.io/) für ein vereinfachtes Fehler-Monitoring. [#183](https://github.com/gcettuzz/chuchipirat/issues/183)
* Upgrade auf Material-UI Version 5. [#126](https://github.com/gcettuzz/chuchipirat/issues/126)
* Wechsel auf Pragmatic Drag and Drop. [#186](https://github.com/gcettuzz/chuchipirat/issues/186)
* Upgrade auf Latest Release-Stände: [#185](https://github.com/gcettuzz/chuchipirat/issues/185)
  * React: **17 → 18.2 → 19.2.x**
  * React Router: **5 → 6 → 7**
  * MUI Material: **v5 → v6 → v7.3.8**
  * Firebase: **10 → 12.9**
  * Tooling: **CRA → Vite**

</details>

---

## 1.0.4 — 24.11.2024

### Fehlerbehebungen

* Navigationsmenü: Beim Eintrag «Anlässe» war nur das Icon als Link klickbar. Der Link wurde auf das ganze Listenelement erweitert. [#153](https://github.com/gcettuzz/chuchipirat/issues/153)
* Rezepte: Wurde nachträglich die Menge eines Materials gelöscht, führte dies unter Umständen zu einem Fehler. [#155](https://github.com/gcettuzz/chuchipirat/issues/155)
* Profil: Das Profil konnte ohne Anzeigenamen gespeichert werden, was beim Erstellen einer Rezeptvariante zu einem Fehler führte. [#156](https://github.com/gcettuzz/chuchipirat/issues/156)
* Skalierung: Fehler bei der Skalierung von Zutaten mit einem Skalierungsfaktor ungleich 1. Die Formel wurde angepasst. [#161](https://github.com/gcettuzz/chuchipirat/issues/161)
* Menüplan: Fehler bei der Anzeige der Total Portionen im Dialog _Für wen planst du das Rezept ein?_, falls eine Einplanung geändert wird und eine Ernährungsgruppe vorausgewählt ist. [#167](https://github.com/gcettuzz/chuchipirat/issues/167)
* Einheitenumrechnung: Bei erfolgloser Umrechnung wird nun zusätzlich versucht, über verwandte Einheiten umzurechnen. [#164](https://github.com/gcettuzz/chuchipirat/issues/164)
* Einkaufsliste: Der Seitenumbruch beim Export führte unter gewissen Umständen zu leeren Seiten. [#166](https://github.com/gcettuzz/chuchipirat/issues/166)
* Registrierung: Einstellungen und Statistikdaten werden erst erzeugt, wenn die E-Mail-Adresse bestätigt wurde. [#172](https://github.com/gcettuzz/chuchipirat/issues/172)
* Rezeptvarianten: Alle Crew-Mitglieder können Rezeptvarianten ändern, nicht nur die Autor\*innen. [#175](https://github.com/gcettuzz/chuchipirat/issues/175)
* Menüplan: Beim Hinzufügen von Produkten wurde teilweise die falsche Einheit übernommen. [#178](https://github.com/gcettuzz/chuchipirat/issues/178)
* Bilder: Beim Hochladen von Bildern wird nun eine Sanduhr angezeigt, bis das Hochladen erfolgreich war. [#181](https://github.com/gcettuzz/chuchipirat/issues/181)

---

## 1.0.3 — 04.05.2024

### Neue Funktionen

* Neuer Menüeintrag `Spenden` — damit kann jederzeit der Twint-Code aufgerufen werden.
* Möglichkeit, Systemmeldungen zu setzen (Admin-Bereich).
* Beim Erfassen eines neuen Produktes wird geprüft, ob es ähnlich klingende Produkte gibt. Eine Liste mit möglichen Übereinstimmungen wird angezeigt, um Doubletten zu vermeiden.

### Verbesserungen

* Passwort-vergessen-Link wird nun bei Falscheingabe des Passwortes angezeigt.
* Möglichkeit, eine Notiz in einem Menü über das Kontextmenü zu löschen.
* Bei der Abmeldung wird das Navigationsmenü nicht mehr angezeigt.
* Auf dem Startbildschirm werden nun mehr Feed-Einträge angezeigt.
* Links in der Fusszeile öffnen sich in einem neuen Tab.

### Fehlerbehebungen

* Fehler im Menüplan beim Hinzufügen von Produkten/Materialien behoben.

---

## 1.0.2 — 15.04.2024

### Verbesserungen

* Erweiterung des klickbaren Bereichs im Navigationsmenü.

### Fehlerbehebungen

* Menüplan: Fehler behoben, bei dem ein Produkt als `undefined` angezeigt wurde.
* Korrektur, um den Text eines Produktes in allen Objekten nachzuziehen.
* Korrektur, um die Quittung einer Spende zu generieren.
* Neues Korrekturprogramm, um falsch erfasste Materialien in Produkte umzuwandeln.
* Neues Korrekturprogramm, um doppelte Materialien zusammenzuführen.

---

## 1.0.1 — 27.03.2024

* Diverse Bugfixes und Layout-Anpassungen.

---

## 1.0.0 — 25.03.2024

* Bereitstellung der App — Go-live!
