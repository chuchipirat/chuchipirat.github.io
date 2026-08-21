# Vorschläge für Dokumentationsverbesserungen

Bitte prüfe die folgenden Textvorschläge. Passe sie an, wo sie inhaltlich nicht korrekt sind. Wenn ein Vorschlag passt, kann ich ihn direkt einbauen.

---

## 1. Technische Begriffe erklären

### UID (in `docs/admin/activate_support_user.md`, `where_used.md`, `mailconsole.md`)

**Aktuell:** UID wird ohne Erklärung verwendet.

**Vorschlag:** Beim ersten Vorkommen erklären:
> die UID (die eindeutige Kennung, die du in der URL des Anlasses findest)

**Stimmt das?** Findet man die UID tatsächlich in der URL?
**Antwort**: ja die UID ist in der URL sichtbar. Sie ist eine crypto.randomUUID().

---

### Cloud Function (in mehreren Admin-Seiten)

**Aktuell:** "Cloud Function" wird häufig verwendet, ohne es zu erklären.

**Vorschlag:** Beim ersten Vorkommen pro Seite ersetzen/ergänzen mit:
> ein automatischer Hintergrundprozess

Oder alternativ: einfach weglassen und nur das Ergebnis beschreiben (z.B. statt "Die Cloud Function aktualisiert alle betroffenen Dokumente" → "Alle betroffenen Einträge werden automatisch aktualisiert").
**Antwort**: Die Cloud Functions wurden mit der letzten Migration entfernt. Diese wurden entfernt. Ist es einfacher für dich, wenn ich dir Zugriff auf das Coding-Projekt gebe oder wenn ich dem anderen Claude.Code sage, er solle Dokumentateion erstellen? Ich habe in beiden Projekten Claude Code amlaufen. Das eine ist die Implementation dieses die Dokumentation.

---

### Skalierungsfaktor (in `docs/recipe/recipe_structure.md`)

**Aktuell:** Wird erwähnt, aber die Erklärung ist abstrakt.

**Vorschlag:** Ein konkretes Beispiel hinzufügen. Aber ich bin unsicher, wie der Skalierungsfaktor im chuchipirat genau funktioniert. Bitte beschreibe mir:
- Was passiert bei Faktor 1 vs. 0.5 vs. 0?
- Welches Beispiel wäre typisch? (z.B. Salz, Öl?)
**Antwort**: Wenn du Skalierungsfaktor meinst, dann hätte ich diese Anwort: Wenn du ein Rezept hochskalierst, werden die Zutaten nicht immer linear skaliert. Beispiel: Wenn du einen Zopf für 6 Personen bäckst, benötigst du 1 kg Mehl und 1 Ei (zum Bestreichen).  Wenn du nun die doppelte Menge zubereitet (also für 12 Personen) benötigst du 2 kg Mehl, aber es reicht nach wie vor 1 Ei. Denn mit dem einen Ei, kannst du bis zu 3 Zöpfe bestreichen. Darum hat das Ei den Skalierungsfaktor 0,3.
---

### Dimension DLS/MAS/VOL (in `docs/masterdata/units.md`)

**Aktuell:** Abkürzungen werden verwendet.

**Vorschlag:** Abkürzungen ausschreiben und Beispiele geben:
> - **Masse** (MAS) — z.B. kg, g
> - **Volumen** (VOL) — z.B. l, dl
> - **Dimensionslos** (DLS) — z.B. Stück, Prise

**Stimmt diese Zuordnung?** 
**Antwort**: ja

---

## 2. Fehlende Einleitungsabsätze

### `docs/event/groupconfiguration.md`

**Aktuell:** Springt direkt in die Konfiguration.

**Vorschlag für einen Einleitungsabsatz (bitte inhaltlich prüfen):**
> Die Mengenberechnung hilft dir, die Portionen für verschiedene Personengruppen korrekt zu berechnen. Das ist besonders nützlich, wenn nicht alle Teilnehmenden bei jeder Mahlzeit dabei sind — zum Beispiel, weil eine Gruppe einen Tagesausflug macht.

**Stimmt das so? Oder wofür wird die Mengenberechnung typischerweise gebraucht?**
**Antwort**: Die Mengenberechnung ist die Konfiguration, wie sich eine Gruppe zusammensetzt. Darin sind alle Essensvorliebeen (Fleisch, Vegetarisch, Vegan usw) sowie Intoleranten (Laktose, Gluten usw.). Diese Matrix definier wieviele Personen von welcher Gruppe am Anlass dabei sind. Die Rezepte werden später einer solchen Gruppe zugeordnet. Dies hat den Vorteil, sollte sich die Gruppengrösse/-zusammensetzung ändern, werden die verknüpften Rezepte automatisch an die neue Anzahl Portionen angepasst. 

---

### `docs/masterdata/unitconversion.md`

**Aktuell:** Springt direkt in die technische Erklärung.

**Vorschlag für einen Einleitungsabsatz (bitte inhaltlich prüfen):**
> Nicht alle Einheiten lassen sich direkt umrechnen. Hier definierst du, wie bestimmte Produkte zwischen Einheiten umgerechnet werden — zum Beispiel, wie viel Gramm eine Dose Kichererbsen enthält.

**Ist das ein gutes Beispiel? Wie wird Einheitenumrechnung im chuchipirat tatsächlich verwendet?**
**Antwort**: Ein besseres Beispiel wäre: Hier definierst du wie schwer ein Esslöffel Honig ist, damit später grosse Mengen gewogen werden können (staht von Hand abgemessen).

---

### `docs/admin/jobs.md`

**Aktuell:** Listet Jobs ohne zu erklären, wann man sie braucht.

**Vorschlag:** Bei jedem Job einen kurzen Hinweis hinzufügen, z.B.:
> Verwende diesen Job, wenn die Startseite falsche Zahlen anzeigt.

**Stimmt das? Wann muss man die Jobs typischerweise ausführen?**
**Antwort**: Diese Seite gibt es nicht mehr. kann gestrichen werden. Im Zusammenhang mit Cloudfunctions.
---

## 3. Rezeptvarianten vs. privates Rezept

### `docs/recipe/recipe_create_variant.md`

**Aktuell:** Erklärt wie man eine Variante erstellt, aber nicht wann man es tun sollte statt ein neues Rezept anzulegen.

**Vorschlag:** Kurzen Vergleich am Anfang hinzufügen. Aber ich brauche deine Hilfe:
- Wann sollte man eine Variante erstellen?
- Wann ist ein neues (privates) Rezept besser?
- Was ist der funktionale Unterschied?
**Antwort**: Eine Variante ist eine temporäre Kopie eines Rezeptes. Sie wird genutzt um für ein Anlass ein Rezept anzupassen (beispielsweise das Rezept laktosefrei zu machen). Die Variante existiert nur innerhalb des Anlasses und kann in einem anderen Anlass nicht wiederverwendet werden. Private Rezepte können nur von dir genutzt werden, sind aber über alle Anlässe verfügbar. 
---

## 4. Release Notes vereinfachen

### `docs/others/release_notes.md`

**Aktuell:** Die Maintenance-Sektion in v1.1.0 listet Framework-Upgrades (Firebase, React, Material-UI) auf, die für Endbenutzer wenig Bedeutung haben.

**Vorschlag:**
- Technische Details in ein einklappbares `<details>`-Element verschieben
- Die Zusammenfassung für Benutzer voranstellen, z.B. "Diverse technische Aktualisierungen für mehr Stabilität und Sicherheit"

**Möchtest du das so?** ja gerne. 

---

## 5. Rollen klarer erklären

### `docs/admin/admin.md`

**Aktuell:** Unterscheidet Community-Leader und System Admin, aber es gibt keine klare Übersicht der Berechtigungen.

**Vorschlag:** Eine einfache Tabelle hinzufügen:

| Funktion | Community-Leader | System Admin |
|----------|:---:|:---:|
| Verfolgungsnachweis | ✅ | ✅ |
| Items Zusammenführen | ✅ | ✅ |
| Rezeptübersicht | ✅ | ✅ |
| Verfolgungsnachweis | ✅ | ✅ |
| Produkt/Material umwandeln | ✅ | ✅ |
| Support User aktivieren | ✅ | ✅ |
| Rezept-Übersicht | ✅ | ✅ |
| Anlässe-Übersicht | ✅ | ✅ |
| Feed-Einträge-Übersicht | ✅ | ✅ |
| Globale Einstellungen | ❌ | ✅ |
| Systemmeldungen | ❌ | ✅ |
| Spendenziel verwalten | ❌ | ✅ |
| Datenintegrität | ❌ | ✅ |
| Mail-Konsole | ❌ | ✅ |
| Migration | ❌ | ✅ |
| Spendenübersicht-Überblick | ❌ | ✅ |
| User-Überblick | ❌ | ✅ |
| Mailbox-Übersicht | ❌ | ✅ |
| Cron-Jobs Übersicht | ❌ | ✅ |



**Kannst du mir die korrekte Zuordnung liefern?** 
**Antwort**: Habe die Tabelle nachgeführt. Es kann sein, dass SEite dazugekommen sind, die es noch nicht gibt. Kannst du in diesem Fall eine Seite hinzufügen, verknüpfen und mit dem Default füllen? Ich führe dann den INhalt nach. 

---

## 6. Allgemeine Helpcenter-Verbesserungen

### A. Glossar-Seite
Vorschlag: Eine neue Seite `docs/others/glossar.md` mit Erklärungen wiederkehrender Begriffe (Anlass, Menüplan, Ernährungsgruppe, Skalierungsfaktor, Community-Leader, etc.). Andere Seiten können dann dorthin verlinken.

### B. Schnellstart-Anleitung
Vorschlag: Eine "Erste Schritte"-Seite, die den typischen Workflow durchgeht: Registrieren → Anlass erstellen → Menüplan planen → Einkaufsliste generieren. Die `index.md` verlinkt bereits auf diese Seiten, aber eine zusammenhängende Anleitung fehlt.

**Wären diese Ergänzungen hilfreich?**
**Antwort**: ja

---

## 7. FAQ-Erweiterung (Entwurf — bitte prüfen)

Folgende Fragen würde ich zur FAQ hinzufügen. Bitte prüfe ob die Antworten korrekt sind:

### "Kann ich ein Rezept aus einem anderen Anlass wiederverwenden?"
> Ja. Alle öffentlichen und deine privaten Rezepte stehen dir in jedem Anlass zur Verfügung. Du kannst sie direkt im Menüplan einplanen. Falls du ein Rezept für einen bestimmten Anlass anpassen möchtest, erstelle eine Rezeptvariante.

**Stimmt das?** ja. Lass uns Rezeptvariant noch verlinken mit der Anleitung create_recipe_variant.md

### "Wie lösche ich einen Anlass?"
> Du kannst einen Anlass in den Anlass-Einstellungen löschen. Achtung: Gelöschte Anlässe können nicht wiederhergestellt werden. 

**Stimmt das? Wo genau löscht man einen Anlass?** ja. auch hier bitte link zu der entsprechenden Seite

### "Warum stimmen die Mengen auf meiner Einkaufsliste nicht?"
> Falls sich die Mengenberechnung oder die Rezepte geändert haben, muss die Einkaufsliste neu generiert werden. Du siehst eine Warnung, wenn die Einkaufsliste nicht mehr aktuell ist.

**Stimmt das?** ja. auch hier ein Link zur Seite Einkaufliste. 

### "Kann ich den chuchipirat auch auf dem Handy nutzen?"
> Ja. Der chuchipirat ist eine Web-App und funktioniert im Browser auf jedem Gerät — Smartphone, Tablet und Computer.

**Stimmt das?** ja

---
//TODO:
## 8. Seiten ohne Screenshots

Folgende Seiten haben keinen Screenshot und würden von einem profitieren:

- `docs/recipe/recipe_create_variant.md` — Wie sieht der "Variante erstellen"-Dialog aus?
- `docs/recipe/recipe_publish.md` — Wie sieht der Veröffentlichungs-Dialog aus?
- `docs/recipe/recipe_report_bug.md` — Wie meldet man einen Fehler im Rezept?
- `docs/request/requests.md` — Wie sieht die Antrags-Übersicht aus?
- `docs/admin/users.md` — User-Übersicht
- `docs/admin/convert_items.md` — Items umwandeln Dialog
- `docs/admin/merge_items.md` — Items zusammenführen Dialog

---

## 9. Seite "Fehler in der App melden" vereinfachen

### Kontext
Mit Sentry (browserTracingIntegration, replayIntegration, Feedback-Formular) werden Browser-Logs, Geräteinformationen und Session-Replays automatisch erfasst. Die gesamte Sektion "Browser-Logs exportieren" und "Zusätzliche Informationen" kann entfallen.

### Vorgeschlagener neuer Inhalt für `docs/others/report_bug.md`

**Bitte prüfe ob der Text korrekt ist, insbesondere:**
- Gibt es in der App tatsächlich ein Sentry-Feedback-Widget/Button? Wo findet der User es?
- Stimmt die E-Mail-Adresse hilfe@chuchipirat.ch noch?
- Ist der Konsistenzcheck-Hinweis noch korrekt?

```markdown
---
layout: home
title: Fehler in der App melden
parent: FAQ
nav_exclude: false
nav_order: 8
permalink: faq/report_bug
---
# Fehler in der App melden
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

{: .important }
> Möchtest du einen **Fehler in einem Rezept** melden (z.B. falsche Mengen oder Zutaten)? Dann nutze die Funktion [Rezept Fehler melden]({% link docs/recipe/recipe_report_bug.md %}).
{::comment}[[recipe_report_bug]]{:/comment}

Die App wurde ehrenamtlich entwickelt. Es wurde grosser Wert auf Richtigkeit und Vollständigkeit gelegt. Dennoch kann nicht garantiert werden, dass die App fehlerfrei ist. Falls du einen Fehler findest, melde diesen, damit sich das chuchipirat-Team darum kümmern kann.

{: .note }
> Betrifft der Fehler die Einkaufs- oder Materialliste oder den Menüplan? Hast du den `Konsistenzcheck` schon ausgeführt? Details dazu findest du [hier]({% link docs/event/event_settings.md %}#menüplan-konsistenzcheck). Wenn der Fehler danach immer noch besteht, melde dich bei uns.
{::comment}[[event_settings]]{:/comment}

## Fehler direkt in der App melden

Der einfachste Weg, einen Fehler zu melden, ist direkt in der App über das Feedback-Formular. [BESCHREIBUNG WO DER USER DAS FEEDBACK-WIDGET FINDET]. Dein Feedback wird zusammen mit hilfreichen technischen Informationen automatisch an uns übermittelt.

## Fehler per E-Mail melden

Alternativ kannst du Fehler an **hilfe@chuchipirat.ch** senden. Beschreibe dabei bitte:

1. **Was ist passiert?** — Beschreibe den Fehler so genau wie möglich.
2. **Wo ist es passiert?** — Auf welcher Seite warst du? (z.B. die URL aus der Adresszeile)
3. **Was hast du gemacht?** — Welche Schritte hast du ausgeführt, bevor der Fehler aufgetreten ist?
4. **Was hättest du erwartet?** — Was hätte stattdessen passieren sollen?

{: .highlight }
> Screenshots oder eine kurze Bildschirmaufnahme helfen uns enorm, den Fehler schnell nachzuvollziehen.

{: .note }
> Aufgrund der ehrenamtlichen Arbeit kann eine längere Bearbeitungszeit auftreten.
```

### Was entfällt und warum
- **"Wie erkenne ich einen Fehler?"** — zu offensichtlich für die meisten User, bläht die Seite auf
- **"Browser-Logs exportieren"** — Sentry erfasst diese automatisch
- **"Zusätzliche Informationen" (OS, Browser, Gerät)** — Sentry erfasst diese automatisch
- **Bilder der Entwicklerkonsole** (`dev_tools.png`, `console_log.png`) — können gelöscht werden wenn die Seite umgeschrieben wird

### Offene Frage
Wo genau findet der User das Sentry-Feedback-Widget in der App? (Button in der Ecke? Menüeintrag? Automatisch bei einem Fehler?) Ich brauche diese Info um den Abschnitt "Fehler direkt in der App melden" korrekt zu formulieren.

**Antwort:** Der Feedbackbutton ist unten rechts als FAB. Ein Megaphon als Icon. Sobald dieser geklickt wird, öffnet sich das Feedbackfesnter. Wenn ein Fehler geschieht, zeigen wir einen Fehlerscreen an mit einem Button der die Seite auffrischt. Dieser Fehlerscreen ist Zeichen dafür, dass der Fehler gemeldet wurde. Dies ist der Text der angezeigt wird: 

Ein unerwarteter Fehler ist aufgetreten. Unsere Crew wurde automatisch benachrichtigt und kümmert sich darum!
Danke für dein Verständnis.

