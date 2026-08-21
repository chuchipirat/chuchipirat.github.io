---
layout: default
title: Mailbox Monitor
permalink: docs/admin/mailbox_overview
nav_exclude: true
parent: System
search_exclude: true
---
# Mailbox Monitor
{: .no_toc }

---

{: .intern-title }
> ☠️ Admin-Bereich ☠️
>
> Diese Seite ist für die System-Admins.

Der Mailbox Monitor zeigt alle E-Mails, die vom chuchipirat versendet wurden. Die Seite hat zwei Tabs: `Übersicht` und `Löschen`.

{: .note }
E-Mails rund um die Authentifizierung (E-Mail bestätigen, Passwort zurücksetzen etc.) werden von GoTrue versendet und erscheinen hier nicht.

![Mailbox](/docs/admin/images/mailbox.png)
## Übersicht

Die Tabelle zeigt alle archivierten E-Mails mit folgenden Spalten:

- **Öffnen:** öffnet die Detailansicht
- **Betreff:** Betreffzeile der E-Mail
- **Nachrichtentext:** Inhalt der E-Mail
- **Empfänger:** E-Mail-Adresse
- **Anzahl Empfänger:** Anzahl der Empfänger\*innen
- **Mail Template:** verwendete Vorlage (z.B. donation-confirmed, newsletter, admin_console, event-review)
- **Status:** z.B. `success`
- **Timestamp:** Zeitpunkt des Versands

Über das Suchfeld kannst du nach bestimmten E-Mails suchen. Die Gesamtanzahl wird oberhalb der Tabelle angezeigt.

### Detailansicht

Klickst du auf das Öffnen-Symbol, siehst du die Details der E-Mail:

- **Betreff:** vollständige Betreffzeile
- **Empfänger:** alle Empfänger\*innen
- **E-Mail-Inhalt:** die an das Template übergebenen Daten (variiert je nach Mail-Typ)

## Löschen

Über den Tab `Löschen` kannst du ältere E-Mail-Protokolle aus der Datenbank entfernen. Gib die Anzahl Tage ein, für die du die Protokolle behalten möchtest, und klicke auf `Mailprotokolle löschen`.
