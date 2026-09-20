---
layout: default
title: Datenintegrität
nav_exclude: true
parent: System
search_exclude: true
---
# Datenintegrität
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
> Diese Seite ist für die System-Admins.

Die Datenintegrität prüft die Konsistenz der Daten im chuchipirat. Über den Button `Alle Prüfungen ausführen` werden alle Prüfungen auf einmal ausgeführt. Alternativ startest du eine einzelne Prüfung mit dem Play-Symbol im jeweiligen Abschnitt.

Jeder Abschnitt zeigt nach der Prüfung ein farbiges Badge:
- **Grün** — keine Auffälligkeiten gefunden
- **Orange** — Einträge gefunden, die überprüft werden sollten

Bei manchen Prüfungen kannst du die gefundenen Einträge direkt bereinigen (siehe unten). Ein Klick auf das Info-Symbol öffnet, wo vorhanden, die Details zum Rezept oder zur Person. Es werden höchstens 50 Einträge aufgelistet. Die Zahl im Badge zeigt aber immer alle gefundenen Einträge.

![Datenintegrität](/docs/admin/images/data_integrity.png)
## Prüfungen

### Events ohne Zeitscheiben

Findet Anlässe, denen kein Zeitraum (keine Zeitscheibe) zugeordnet ist. Solche Anlässe entstehen zum Beispiel, wenn das Anlegen eines Anlasses unterbrochen wird, bevor die Daten gespeichert sind.

Zu jedem Anlass siehst du, ob er **leer** ist oder **Daten enthält**, wer ihn wann angelegt hat, wann er zuletzt geändert wurde und wie viele Köch\*innen, Mahlzeiten, Listen und Spenden dazugehören. So erkennst du, ob es sich um einen abgebrochenen Entwurf oder um einen echten Anlass handelt, bei dem die Zeiträume verloren gegangen sind.

- **Einzelnen Anlass löschen:** Über das Papierkorb-Symbol löschst du jeden Anlass, auch einen mit Inhalt. Der Bestätigungsdialog nennt dir den Inhalt noch einmal.
- **Leere Anlässe löschen:** Der Button `N leere löschen` löscht alle Anlässe, die leer sind. Anlässe mit Inhalt bleiben stehen und müssen einzeln gelöscht werden.

{: .warning }
Beim Löschen eines Anlasses wird alles gelöscht, was dazugehört: Menüplan, Einkaufs- und Materiallisten, Notizen und Köch\*innen. Das lässt sich nicht rückgängig machen. Ein Anlass gilt nur als leer, wenn er keine Mahlzeiten, keine Listen und keine verknüpfte Spende hat.

{: .note }
Hat ein Anlass inzwischen doch eine Zeitscheibe bekommen, wird er nicht gelöscht. Du siehst dann die Meldung «Nicht gelöscht», und die Prüfung wird neu geladen.

### Events ohne Köch\*innen

Findet Anlässe, bei denen niemand als Koch oder Köchin eingetragen ist. Solche Anlässe sind für normale Nutzer\*innen in der Regel nicht mehr sichtbar und können deshalb nicht selbst aufgeräumt werden. Anzeige und Löschen funktionieren wie bei «Events ohne Zeitscheiben».

### Unbenutzte Produkte

Listet Produkte auf, die in keinem Rezept, keiner Einkaufsliste, keiner Menüplanung und keiner Einheitenumrechnung referenziert werden. Sie können einzeln oder mit `Alle N löschen` bereinigt werden. Bevor du löschst, lohnt sich ein Blick in den [Verfolgungsnachweis]({% link docs/admin/where_used.md %}).
{::comment}[[where_used]]{:/comment}

### Unbenutzte Materialien

Listet Materialien auf, die in keinem Rezept, keiner Materialliste und keiner Menüplanung referenziert werden. Sie können einzeln oder mit `Alle N löschen` bereinigt werden.

### Rezepte ohne Event

Zeigt öffentliche Rezepte, die in keinem Menüplan eines Anlasses verwendet werden. Über das Info-Symbol siehst du die Details des Rezepts. Löschen ist einzeln oder mit `Alle N löschen` möglich.

### Rezept-Zutaten ohne Produkt

Findet Rezepte, in denen eine Zutat kein Produkt hat. Das passiert, wenn ein Produkt gelöscht wurde, das in einem Rezept noch vorkam, oder wenn beim Erfassen nur eine Menge, aber kein Produkt gewählt wurde. Menge, Einheit und Detailangabe der Zeile bleiben erhalten, nur der Name des Produkts fehlt.

Zu jedem Rezept siehst du den Typ (öffentlich, privat oder Variante), wer es erstellt hat und die betroffenen Zeilen, zum Beispiel «500 g (frisch)». Da der Name des gelöschten Produkts nicht mehr bekannt ist, helfen dir Menge, Einheit und Detailangabe beim Erkennen.

{: .important }
Ein Rezept mit einer Zutat ohne Produkt kann die Erstellung der Einkaufsliste eines Anlasses stören. Bereinige diese Rezepte deshalb zeitnah.

So behebst du es:
1. Klicke auf das Symbol `Rezept öffnen`.
2. **Öffentliche Rezepte und Varianten** kannst du als Admin bearbeiten: Wähle bei der betroffenen Zutat ein Produkt und speichere das Rezept.
3. **Private Rezepte** kann nur die Person bearbeiten, die sie erstellt hat. Schreibe ihr über die [Mail-Konsole]({% link docs/admin/mailconsole.md %}).
{::comment}[[mailconsole]]{:/comment}

Diese Prüfung ist nur eine Anzeige, es wird nichts automatisch gelöscht.

### Rezept-Materialien ohne Material

Findet Rezepte mit Materialpositionen, denen kein Material zugeordnet ist. Das passiert, wenn ein Material gelöscht wurde, das in einem Rezept noch vorkam, oder wenn eine leere Zeile gespeichert wurde. Die Anzeige und das Beheben funktionieren wie bei den Zutaten. Zeilen ohne Material entfernt der Rezept-Editor beim Speichern automatisch: Rezept öffnen, bearbeiten und speichern genügt bei öffentlichen Rezepten und Varianten. Nur Anzeige, gelöscht wird nichts automatisch.

### Benutzer ohne Event

Listet Benutzer\*innen, die bei keinem Anlass als Koch oder Köchin eingetragen sind. Über das Info-Symbol siehst du die Details der Person. Diese Prüfung ist nur eine Anzeige, hier wird nichts gelöscht.

### Doppelte E-Mail-Adressen

Findet Benutzer\*innen, die dieselbe E-Mail-Adresse haben (Gross- und Kleinschreibung spielt keine Rolle). Nur Anzeige.

## Sicherheitsnetze

Die folgenden drei Prüfungen finden normalerweise nichts, weil die Datenbank die Fehler schon beim Speichern verhindert. Sie bleiben als Sicherheitsnetz erhalten, falls sich daran einmal etwas ändert. Erscheint hier trotzdem ein Eintrag, melde das bitte an die Entwicklung.

- **Verwaiste Rezepte:** Rezepte, deren Ersteller nicht mehr existiert.
- **Verwaiste Event-Köche:** Koch-Einträge, die keinem bestehenden Anlass mehr zugeordnet sind.
- **Auth/Users Sync:** Benutzer\*innen ohne passenden Eintrag im Anmeldesystem.
