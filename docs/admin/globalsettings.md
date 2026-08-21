---
layout: default
title: Globale Einstellungen
nav_exclude: true
parent: System
search_exclude: true
---
# Globale Einstellungen
{: .no_toc }

---

{: .intern-title }
> ☠️ Admin-Bereich ☠️
>
> Diese Seite ist für die System-Admins.

In den globalen Einstellungen kannst du systemweite Funktionen konfigurieren. Um Änderungen vorzunehmen, klicke zuerst auf `Anpassen` und nach der Anpassung auf `Speichern`.

![Globale Einstellungen](/docs/admin/images/global_settings.png)
## Neu-Anmeldung ermöglichen

Steuert, ob neue Konten im chuchipirat erstellt werden können (Neuanmeldung/Registrierung). Bestehende Benutzer\*innen können sich unabhängig von dieser Einstellung weiterhin anmelden.

## Wartungsmodus

Im Wartungsmodus ist weder eine Anmeldung noch eine Neuregistrierung möglich.

## E-Mail-Suche Rate-Limit

Legt die maximale Anzahl E-Mail-Suchen pro Benutzer\*in pro Stunde fest.

## E-Mails an MailPit umleiten

Wenn aktiviert, werden alle App-E-Mails (Cron-Jobs, Benachrichtigungen) an MailPit gesendet statt an echte Empfänger\*innen. Nützlich für Tests. Davon ausgenommen sind alle E-Mails rund um Authentifizierung (E-Mailadresse bestätigen, E-Mailadresse wechseln, Passwort vergessen).

## Alle Benutzer\*innen abmelden

Über `Alle abmelden` werden alle angemeldeten Benutzer\*innen vom chuchipirat abgemeldet — ausser solche mit der Admin-Rolle.

{: .important }
Es kann bis zu einer Stunde dauern, bis alle Benutzersitzungen beendet sind.
