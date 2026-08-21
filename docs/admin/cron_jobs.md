---
layout: default
title: Cron-Jobs Übersicht
nav_exclude: true
parent: System
search_exclude: true
---
# Cron-Jobs Übersicht
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

Die Cron-Jobs-Übersicht ist ein Cockpit zur Überwachung der geplanten Hintergrund-Jobs. Hier siehst du, ob die Jobs erfolgreich ausgeführt wurden, und kannst sie bei Bedarf manuell erneut starten.

![Übersicht Cron Jobs](/docs/admin/images/cron_jobs.png)

## Jobs

### cron-daily-digest

Sendet täglich eine Zusammenfassung per E-Mail an alle Community-Leader. Das Digest enthält Informationen über die letzten 24 Stunden:

- Neu registrierte Nutzer\*innen
- Neu erstellte Anlässe
- Neu erstellte Rezepte
- Neu erfasste Produkte und Materialien
- Neue Rezeptkommentare
- Zusammenfassung verschiedener Aktionen (Feed-Einträge)

Ziel ist, dass Community-Leader auf einen Blick erkennen, ob Handlungsbedarf besteht: z.B. falsch kategorisierte Produkte oder unangemessene Kommentare.

### cron-support-user-cleanup

Das Gegenstück zur Funktion [Support-User aktivieren]({% link docs/admin/activate_support_user.md %}). Dieser Job entfernt den Support-User automatisch von allen Anlässen. Falls die Support-Arbeit noch nicht abgeschlossen ist, muss der Support-User erneut aktiviert werden.
{::comment}[[activate_support_user]]{:/comment}

### cron-event-review-email

Sammelt alle Anlässe, die am Vortag geendet haben, und sendet eine E-Mail an alle Köch\*innen des Anlasses. Die E-Mail fragt, wie der Anlass gelaufen ist, bittet um Feedback und weist auf die Möglichkeit hin, dem chuchipirat eine Spende zukommen zu lassen.

### cron-housekeeping

Wöchentlicher Aufräum-Job, der veraltete Daten aus verschiedenen Tabellen entfernt. Folgende Bereinigungen werden durchgeführt:

| Aufgabe | Aufbewahrungsfrist |
|---|---|
| Alte Feed-Einträge | 12 Monate |
| Alte Cron-Job-Logs | 90 Tage |
| Alte Mail-Logs | 90 Tage |
| pg_cron-Verlauf | 90 Tage |
| Abgebrochene Spenden (Status «pending») | 7 Tage |
| Fehlgeschlagene/abgebrochene Spenden | 90 Tage |
| Abgelaufene Systemmeldungen | 30 Tage nach Ablauf |

## Übersicht

Die Tabelle zeigt alle Job-Ausführungen mit folgenden Spalten:

- **Job** — Name des Cron-Jobs
- **Gestartet** — Zeitpunkt der Ausführung
- **Dauer (ms)** — Dauer in Millisekunden
- **Status** — `success`, `running` oder `error`
- **Verarbeitet** — Anzahl verarbeiteter Einträge
- **Fehler** — Fehlermeldung (falls vorhanden)
- **Details** — Link zur JSON-Ausgabe des Jobs

Über den **Job-Filter** kannst du die Tabelle auf einen bestimmten Job einschränken.

## Jobs manuell ausführen

Über die Buttons `Cron-Daily-Digest`, `Cron-Support-User-Cleanup` und `Cron-Event-Review-Email` oberhalb der Tabelle kannst du einen Job manuell starten. Das ist nützlich, wenn ein Job fehlgeschlagen ist und erneut ausgeführt werden soll.
