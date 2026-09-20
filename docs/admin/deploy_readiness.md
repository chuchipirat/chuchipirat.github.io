---
layout: default
title: Deploy-Check
nav_exclude: true
parent: System
search_exclude: true
---
# Deploy-Check
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

Der Deploy-Check zeigt dir, ob du gerade eine neue Version des chuchipirat veröffentlichen (deployen) kannst, ohne jemanden bei der Arbeit zu stören. Beim Veröffentlichen werden laufende Verbindungen kurz getrennt: Wer gerade etwas bearbeitet, kann Änderungen verlieren oder muss die Seite neu laden.

![Deploy-Check](/docs/admin/images/deploy_readiness.png)

## Die zwei Kennzahlen

Ganz oben siehst du zwei Kacheln:

- **Lager heute** — Anzahl der Anlässe, die heute laufen.
- **Aktiv in den letzten 15 Minuten** — Anzahl der Personen, die in den letzten 15 Minuten etwas geändert haben. Jede Person wird nur einmal gezählt, auch wenn sie an mehreren Orten arbeitet.

Eine Kachel ist grün, wenn der Wert 0 ist, und rot, wenn er grösser als 0 ist. Sind beide grün, ist ein guter Moment für ein Deploy.

## Laufende Lager

Hier stehen alle Anlässe, bei denen das heutige Datum in einem der erfassten Zeiträume liegt. Mit einem Klick auf einen Anlass öffnest du ihn.

{: .important }
Während ein Lager läuft, solltest du nicht deployen. Dann kochen die Leute mit der App und brauchen sie ohne Unterbruch, oft auf dem Handy und ohne stabile Verbindung.

## Letzte Aktivität

Die Liste zeigt, wer in den letzten 24 Stunden wo etwas geändert hat. Pro Person und Objekt siehst du die letzte Änderung, die neuste zuoberst:

- **Person** — Wer hat etwas geändert? «System» steht für automatische Vorgänge ohne Person, zum Beispiel geplante Jobs.
- **Bereich** — Anlass, Rezept, Stammdaten oder Anfrage.
- **Objekt** — Name des Anlasses, Rezepts oder der Stammdaten.
- **Letzte Änderung** — Wie lange die Änderung her ist («vor 7 Min.»). Wenn du mit der Maus darüberfährst, siehst du die genaue Uhrzeit.

Änderungen der letzten 15 Minuten sind farbig hervorgehoben. Auf dem Handy siehst du statt der Tabelle einzelne Karten.

{: .highlight }
Viele Teams planen ihr Lager lange im Voraus. Deshalb erscheinen in der Liste auch Anlässe, die erst in ein paar Monaten stattfinden. So erkennst du auch dann Aktivität, wenn gerade kein Lager läuft.

## Aktualisierung

Die Seite lädt sich alle 30 Sekunden selbst neu. Mit dem Button **Aktualisieren** holst du die neusten Daten sofort. Neben dem Button siehst du, wann zuletzt geladen wurde.

## Was die Seite nicht zeigt

- **Wer nur liest:** Angezeigt werden nur Änderungen (auch neu Angelegtes). Wer ein Rezept nur anschaut oder eine Einkaufsliste nur liest, erscheint nicht in der Liste.
- **Gelöschtes:** Wird etwas gelöscht, bleibt keine Spur zurück.

{: .note }
Der Deploy-Check ist eine Entscheidungshilfe. Ob du deployst, entscheidest du. Ist die Aktivitätsliste leer, aber dir ist bekannt, dass jemand gerade kocht, ist im Zweifel Warten die bessere Wahl.
