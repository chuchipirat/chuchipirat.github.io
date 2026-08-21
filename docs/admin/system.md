---
layout: default
title: System
nav_exclude: true
has_children: true
nav_order: 9
search_exclude: true
---
# System
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
> Die folgenden Seiten sind für die Community-Leader\*innen und System-Admins.

## Berechtigungen

| Funktion                   | Community-Leader | System Admin |
| -------------------------- | :--------------: | :----------: |
| Einheiten                  |        ✅         |      ✅       |
| Verfolgungsnachweis        |        ✅         |      ✅       |
| Items zusammenführen       |        ✅         |      ✅       |
| Rezept-Übersicht           |        ✅         |      ✅       |
| Produkt/Material umwandeln |        ✅         |      ✅       |
| Support User aktivieren    |        ✅         |      ✅       |
| Anlässe-Übersicht          |        ✅         |      ✅       |
| Feed-Einträge-Übersicht    |        ✅         |      ✅       |
| Spendenübersicht           |        ✅         |      ✅       |
| Globale Einstellungen      |        ❌         |      ✅       |
| Systemmeldungen            |        ❌         |      ✅       |
| Spendenziel verwalten      |        ❌         |      ✅       |
| Datenintegrität            |        ❌         |      ✅       |
| Mail-Konsole               |        ❌         |      ✅       |
| User-Überblick             |        ❌         |      ✅       |
| Mailbox-Übersicht          |        ❌         |      ✅       |
| Cron-Jobs Übersicht        |        ❌         |      ✅       |

## Einstellungen

- [Globale Einstellungen]({% link docs/admin/globalsettings.md %}) — den chuchipirat in den Wartungsmodus stellen und Neuanmeldungen verhindern
- [Systemmeldungen]({% link docs/admin/system_message.md %}) — systemweite Meldungen erstellen und verwalten
- [Spendenziele verwalten]({% link docs/admin/donation_goal.md %}) — Spendenziele für den chuchipirat konfigurieren
- [Einheiten]({% link docs/admin/units.md %}) — Anpassen und Ergänzen von Einheiten
{::comment}[[globalsettings]][[system_message]][[donation_goal]][[units]]{:/comment}

## Datenoperationen

- [Verfolgungsnachweis]({% link docs/admin/where_used.md %}) — Produkte und Materialien in Rezepten aufspüren, quer durch die gesamte Applikation
- [Items zusammenführen]({% link docs/admin/merge_items.md %}) — gleiche Produkte oder Materialien zu einem zusammenführen
- [Items umwandeln]({% link docs/admin/convert_items.md %}) — ein Produkt in ein Material umwandeln und alle betroffenen Objekte anpassen
- [Support-User aktivieren]({% link docs/admin/activate_support_user.md %}) — den Support-User einem Anlass hinzufügen, um Support leisten zu können
- [Datenintegrität]({% link docs/admin/data_integrity.md %}) — Konsistenz der Daten prüfen (verwaiste Rezepte, unbenutzte Produkte etc.)
- [Mail-Konsole]({% link docs/admin/mailconsole.md %}) — E-Mails an Benutzer\*innen versenden
- [Anträge bearbeiten]({% link docs/admin/handle_recipe_request.md %}) — eingereichte Anträge (Rezeptfreigabe, Fehlermeldungen) prüfen und bearbeiten
{::comment}[[where_used]][[merge_items]][[convert_items]][[activate_support_user]][[data_integrity]][[mailconsole]][[handle_recipe_request]]{:/comment}

## Übersichten

- [Übersicht Rezepte]({% link docs/admin/recipe_overview.md %}) — Übersicht aller Rezepte, privat wie öffentlich
- [Übersicht Anlässe]({% link docs/admin/event_overview.md %}) — Übersicht aller erfassten Anlässe
- [Übersicht Feed-Einträge]({% link docs/admin/feed_overview.md %}) — Übersicht aller generierten Feed-Einträge
- [Spendenübersicht]({% link docs/admin/donation_overview.md %}) — Übersicht aller eingegangenen Spenden
- [User-Überblick]({% link docs/admin/users.md %}) — Übersicht aller Benutzer\*innen
- [Mailbox-Übersicht]({% link docs/admin/mailbox_monitor.md %}) — Übersicht über alle versendeten E-Mails
{::comment}[[recipe_overview]][[event_overview]][[feed_overview]][[donation_overview]][[users]][[mailbox_monitor]]{:/comment}

## Cron Jobs

- [Cron-Jobs Übersicht]({% link docs/admin/cron_jobs.md %}) — Überwachung und manuelle Ausführung der geplanten Hintergrund-Jobs
{::comment}[[cron_jobs]]{:/comment}
