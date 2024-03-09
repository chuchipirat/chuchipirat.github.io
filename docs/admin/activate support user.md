---
layout: home
title: Support-User aktivieren
permalink: docs/admin/activate_support_user
nav_exclude: 
parent: System
search_exclude: true
---
# Support User aktivieren
{: .no_toc }

## Inhalt
{: .no_toc .text-delta }

- TOC
{:toc}

---

{: .intern-title }

> ☠️ Admin-Bereich ☠️
>
>Diese Seite ist für die Community-Leader\*innen und System-Admins.

Auch als Community-Leader\*in oder Admin hast du keinen Zugriff auf die Anlässe anderer Nutzer. Um jedoch im Supportfall Hilfe leisten zu können, steht dir die Funktion «Support-User aktivieren» zur Verfügung. Mit dieser Option kannst du den Support-User für ein bestimmtes Ereignis autorisieren. Die Berechtigung wird automatisch um 01:00 Uhr morgens zurückgesetzt.


![Support-User aktivieren](https://github.com/chuchipirat/chuchipirat.github.io/blob/main/docs/admin/_images/activate_support_user.png?raw=true)

## Vorgehen

1. Trage die Event-UID in das entsprechende Feld ein und klicke auf `Support-Modus aktivieren`.
2. Hinter den Kulissen wird eine Cloud-Function gestartet, die den Support-User für das angegebene Ereignis autorisiert.
3. Falls das angegebene Ereignis nicht existiert, erhältst du eine entsprechende Fehlermeldung.
4. Logge dich mit dem Support-User ein. Damit kannst du nun auf das angegebene Ereignis zugreifen.

{: .note }
> Beachte: Die Berechtigung für den Support-User wird automatisch um 01:00 Uhr zurückgesetzt. Solltest du danach erneut darauf zugreifen müssen, wiederhole einfach die Schritte 1–4.